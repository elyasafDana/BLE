# AdPlusScan - Android BLE Scanner & Advertiser

This app is built with Java and lets an Android phone act as both a BLE Scanner (finding devices) and a BLE Advertiser (broadcasting its presence) at the same time.

> [!NOTE]
> **Project Status:** This is a core part of a larger, more complex system I am currently developing.

---

## 🚀 Key Features

* **BLE Advertising (Peripheral Mode):** The phone sends out signals with a unique ID (UUID) and custom manufacturer data that I defined.
* **BLE Scanning (Central Mode):** The app actively looks for nearby devices, showing their ID (UUID) and how strong the signal is (RSSI).
* **Smart Permissions:** I built a system to handle Android’s tricky permissions (like Location and Bluetooth) in real-time so the app runs smoothly without crashing. The application performs real-time permission checks and automatically prompts the user for the required authorizations.

---

## 🛠 Tech Stack

* **Language:** Java.
* **Android SDK:** Bluetooth LE APIs (BluetoothLeScanner, BluetoothLeAdvertiser).
* **UI:** Material Design with Edge-to-Edge support.
* **Version Control:** Git & GitHub.

While debugging was primarily conducted on a legacy device—where location access encompasses BLE functionality—the codebase is fully equipped to handle the granular permissions required by modern Android versions.

---

## 📋 How to Run the Project

1. **Clone the repo:** `git clone https://github.com/Adi052447/AdPlusScan.git`
2. **Open in Android Studio.**
3. **Use a real phone:** BLE doesn't work well on emulators. Make sure your Bluetooth and Location are turned on.
4. **Run the app:** Click "Scan" to find devices or "Advertise" to let others find you.

---

## Summary
This project shows my ability to work directly with phone hardware, handle complex Android permissions, and write clean, asynchronous code.
