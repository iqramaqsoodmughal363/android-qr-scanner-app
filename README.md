# 📷 QR Scanner App

<p align="center">
  <b>Scan, Save, and Manage your QR Codes effortlessly.</b>
</p>

<p align="center">
  <em>"A fast and reliable Android application built in Java to scan QR codes and barcodes, featuring a built-in history to keep track of your past scans."</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F-red" alt="Made with Love">
  <img src="https://img.shields.io/badge/Platform-Android-green" alt="Platform">
  <img src="https://img.shields.io/badge/Language-Java-orange" alt="Language">
  <img src="https://img.shields.io/badge/Feature-QR%20Scanning-blueviolet" alt="Feature">
  <img src="https://img.shields.io/badge/Status-Complete-success" alt="Status">
</p>

---

## 📋 Overview

**QR Scanner App** is a lightweight, efficient, and user-friendly Android application. Built entirely in **Java**, it utilizes your device's camera to instantly scan QR codes and barcodes. 

A standout feature of this app is its **Scan History**. Every time you scan a code, it is saved locally so you can easily view, copy, or refer back to it later without having to scan it again.

---

## ✨ Key Features

* **📸 Instant Scanning (`ScannerActivity.java`):** Quickly scan QR codes and barcodes using the device camera.
* **📜 Scan History (`MainActivity.java` & `HistoryAdapter.java`):** View a detailed list of all previously scanned codes.
* **📋 Easy Access:** Easily view the decoded text or link from your past scans.
* **🎨 Clean UI:** Simple, intuitive layouts (`activity_main.xml`, `activity_scanner.xml`) designed for a seamless user experience.
* **🌙 Theme Support:** Includes support for different screen densities and themes (values, values-night, etc.).

---

## 🛠️ Tech Stack

| Category | Tools / Technologies |
|---|---|
| **Language** | Java |
| **IDE** | Android Studio |
| **Camera API** | CameraX / ZXing (Barcode Scanning) |
| **UI Components** | XML Layouts, RecyclerView (for History) |
| **Data Storage** | Local Storage (SQLite / SharedPreferences) |

---

## 📂 Project Structure

```text
android-qr-scanner-app/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/whatsapp/qrscannerapp/
│   │   │   │   ├── HistoryAdapter.java       # RecyclerView Adapter for scan history
│   │   │   │   ├── MainActivity.java         # Dashboard & History Display
│   │   │   │   └── ScannerActivity.java      # Camera view & QR decoding logic
│   │   │   ├── res/
│   │   │   │   ├── drawable/                 # Icons and backgrounds
│   │   │   │   ├── layout/                   # UI Layouts
│   │   │   │   │   ├── activity_main.xml
│   │   │   │   │   └── activity_scanner.xml
│   │   │   │   ├── menu/                     # Options menu
│   │   │   │   ├── mipmap-*/                 # App launcher icons
│   │   │   │   ├── navigation/               # Navigation graph (if using Jetpack)
│   │   │   │   ├── values/                   # Colors, Strings, Themes
│   │   │   │   ├── values-night/             # Dark mode themes
│   │   │   │   └── xml/                      # Backup rules
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   ├── proguard-rules.pro
│   └── gradle/
├── build.gradle
├── settings.gradle
└── README.md
```

---

## 🚀 How to Build and Run

### Prerequisites
* **Android Studio** (Latest Version)
* **JDK 11** or higher
* **Android SDK** (API 21+)
* **Physical Device Recommended:** (Cameras work best on real devices, though emulators can simulate them).

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/iqramaaqsoodmughal363/android-qr-scanner-app.git
   ```
2. **Open in Android Studio**
   Open Android Studio → **File** → **Open** → Select the `QRScannerApp` folder.
3. **Sync Gradle**
   Wait for Gradle to sync. Click **"Sync Now"** if prompted.
4. **Build and Run**
   Connect your Android device, grant camera permissions, and click the **Run** button (green play icon).

---

## ⚙️ How It Works (Behind the Scenes)

### 1. The Scanning Engine (`ScannerActivity.java`)
This activity initializes the device camera. It uses a scanning library (like ZXing or ML Kit) to analyze the camera frames in real-time. Once a QR code is detected, it extracts the string data, stops the camera, and saves the result.

### 2. History Management (`MainActivity.java` & `HistoryAdapter.java`)
After a successful scan, the data is saved locally. The `MainActivity` uses a `RecyclerView` along with the `HistoryAdapter` to display these saved results in a clean list format. 

### 3. Permissions
The app requires `android.permission.CAMERA` to function. The app handles runtime permissions gracefully, asking the user for access upon opening the scanner.

---

## 🎯 Key Takeaways

* **Practical Utility:** A real-world application that solves an everyday problem.
* **Camera Integration:** Demonstrates how to use hardware features (camera) in Android.
* **Data Persistence:** Shows how to save and retrieve data locally for a history feature.
* **Clean Java Code:** Well-structured Activities and Adapters.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**

*Software Engineer · Full-Stack Developer · Code Craftsman · Android App Developer · Problem Solver 🚀*

```javascript
const codeIsLife = "Code is life";
while (true) { 
    learn(); 
    build(); 
    innovate(); 
}
```

---

## 📅 Date

October 26, 2026

---

## 📄 License

This project is intended for educational and personal use purposes.
