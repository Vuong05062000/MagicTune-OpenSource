# MagicTune Tool (Open Source)

MagicTune Tool is an open-source Android utility built with Jetpack Compose, Wireless ADB (`libadb-android`), Shizuku, Material 3, and ML Kit, designed for Honor MagicOS and modern Android devices.

> **Project Status:** This project is no longer commercialized and is now fully open-sourced under the [MIT License](LICENSE). Thank you to everyone who supported the project in the past!

---

## Features / Tính năng chính

- **Wireless ADB & Shizuku Bridge:** On-device NSD WLAN ADB pairing & shell execution without a PC.
- **Home Screen Widgets:**
  - 3×2 & 2×2 Live Battery Widgets (charging wattage, mAh drain analytics, Bluetooth device battery rings, cycle count toggle)
  - App Search & Gesture Draw Widget (recent apps + handwriting app launcher)
  - RAM & ROM Optimizer Widget
  - Clock, Weather & 24h/7d Forecast Widget + Perpetual Lunar Calendar Widget
  - Global widget background transparency slider (0%–100%)
- **Notification & OEM Tuning:** Background keep-alive tuning for Android / Honor / Xiaomi / OPPO / Vivo / Samsung.
- **AI & Screen Utilities:** On-device ML Kit OCR screen translator, Circle-to-Search overlay, gesture letter app launcher, and thermal ESC/POS printer support (K80 / K57 via LAN/Wi-Fi/Bluetooth).
- **In-App Updater:** Supports APK updates hosted on **GitHub Releases** or **Google Drive**.

---

## Tech Stack

- **Language:** Kotlin, Jetpack Compose (Material 3)
- **Min / Target / Compile SDK:** `24` / `36` / `36`
- **Build System:** Gradle `9.3.1`, Android Gradle Plugin `9.1.1`, Java `17+`
- **Core Libraries:** `libadb-android`, `conscrypt-android`, Shizuku API, ML Kit Text Recognition, Firebase (optional)

---

## Getting Started / Hướng dẫn build

1. **Prerequisites:** JDK 17 or 21, Android SDK Platform 36, Build-Tools `36.0.0`.
2. Create `local.properties` in the project root:
   ```properties
   sdk.dir=/path/to/Android/Sdk
   ```
3. *(Optional)* Copy `private.properties.example` to `private.properties`, `keystore.properties.example` to `keystore.properties`, and `google-services.json.example` to `google-services.json` if you want Firebase/release signing.
4. **Build Debug APK:**
   ```bash
   # macOS / Linux
   ./gradlew assembleDebug

   # Windows
   gradlew.bat assembleDebug
   ```

---

## License

Released under the [MIT License](LICENSE). Anyone worldwide is free to use, modify, fork, and distribute this project.
