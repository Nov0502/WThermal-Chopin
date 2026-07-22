# 🌡️ WThermal Chopin (v1.0.0)

**WThermal Chopin** is an intelligent dynamic thermal management module specifically designed for **POCO X3 GT / Redmi Note 10 Pro 5G (`chopin`)** powered by the **MediaTek Dimensity 1100** processor.

Created by: **Nov0502**

---

## 🌟 Key Features

* 🔓 **Default Unthrottled Performance**: Disables Xiaomi thermal throttling daemons (`mi_thermald`, `thermal_manager`, `thermalload`, `thermald`) and locks performance mode (`sconfig 10`) for maximum FPS during gaming.
* 🛡️ **Intelligent Thermal Safety Guard**: Monitors hardware temperatures every 2 seconds and automatically re-enables thermal protection if safety thresholds are breached:
  * 🔴 **Limit Active**: Triggered if CPU $\ge 78^\circ\text{C}$ **OR** Battery $\ge 49^\circ\text{C}$.
  * 🟢 **Release Unthrottled**: Restored when CPU $< 75^\circ\text{C}$ **AND** Battery $< 46^\circ\text{C}$.
* 📊 **Native Ongoing Status Notification**: Bundles a lightweight Foreground Service APK (`WThermalNotifier.apk`) to display live real-time CPU & Battery temperature tracking directly in your notification shade:
  ```text
  WThermal Chopin
  CPU: 42°C  |  Batt: 36°C  |  🟢 UNTHROTTLED
* 📱 MediaTek Dimensity 1100 Dynamic Sensor Engine: Features dynamic case-insensitive MTK thermal zone discovery for accurate temperature reporting across all custom kernels.
* 📝 Real-time Logging System: Logs all temperature transitions to /sdcard/wthermal.log for instant verification.

---

## 🛠️ Supported Environments
Device: POCO X3 GT / Redmi Note 10 Pro 5G (chopin) (just try)
SoC: MediaTek Dimensity 1100 (MT6891)
ROM: MIUI 12.5 / 13 / 14 / HyperOS / AOSP (Android 11 - 14)

---

## 🚀 Installation Guide
1. Download WThermal_Chopin.zip.
2. Open your Root Manager (SukiSU, KernelSU, Magisk, or APatch).
3. Select Install from Storage / Modules and select WThermal_Chopin.zip.
4. Reboot your device.

---

🔍 How to Verify Live Logs
Open Termux or any root file manager and view the live event log:
sh
```text
cat /sdcard/wthermal.log
```

**Author**: @Nov0502
lol
