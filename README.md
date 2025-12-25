
# BLE Advertising & Scanning – Android Implementation

This Android application, developed in **Java**, provides a robust implementation of **Bluetooth Low Energy (BLE)** communication. It bridges the gap between high-level UI actions and low-level hardware interaction, demonstrating a deep understanding of the BLE protocol and Android system architecture.

> [!NOTE]
> **Project Status:** This module is a core functional subsystem of the **"Lost-Found"** project, currently under active development.

---

## 🛠 Technical Highlights

### BLE Architecture & Hardware Interaction
The project manages the dual-role lifecycle of a BLE device:
* **Peripheral Role (Advertising):** Constructs and broadcasts BLE packets containing **Service UUIDs** and **Manufacturer-specific data**.
* **Central Role (Scanning):** Actively discovers nearby peripherals, parsing scan results to extract **RSSI** (signal strength), device names, and advertised payloads.
* **Hardware Awareness:** Implements defensive checks for Bluetooth availability and **Multiple Advertisement** support to ensure stability across different hardware capabilities.

### Android System Integration
* **Dynamic Permission Engine:** A comprehensive flow for handling **Runtime Permissions** required for BLE. The system detects and reacts to missing, denied, or permanently denied states to maintain a smooth user experience.
* **Lifecycle-Conscious Logic:** Uses **Handlers** and **Callbacks** (`ScanCallback`, `AdvertiseCallback`) to manage time-limited scanning windows, preventing unnecessary battery drain and memory leaks.

---

## 🚀 Key Features

* **BLE Advertising:**
    * Customizable Service UUIDs.
    * Injection of Manufacturer-specific payloads.
    * Configurable broadcasting parameters.
* **BLE Scanning:**
    * Real-time extraction of RSSI and device metadata.
    * Packet parsing for Service UUIDs and raw data.
* **Robust Error Handling:** Extensive logging and validation for every step of the BLE workflow.

---

## 💻 Technology Stack

| Component | Technology |
| :--- | :--- |
| **Language** | Java |
| **Platform** | Android SDK |
| **Communication** | Bluetooth Low Energy (BLE) |
| **Database** | Integration with Firebase/Firestore (In Progress) |

---

## 📋 Requirements & Setup

1. **Hardware:** A physical Android device with BLE support (emulators are not supported for BLE features).
2. **Configuration:** Bluetooth must be enabled on the device.
3. **Permissions:** The app will request Location/Bluetooth permissions at runtime to access hardware radio.

---

## 🎯 Purpose
This project serves as a technical showcase of practical Android development, focusing on system-level APIs, asynchronous programming, and real-world hardware constraints. It reflects a solid foundation in building non-trivial mobile features that interact directly with device sensors.
