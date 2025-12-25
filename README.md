BLE Advertising & Scanning – Android App
Overview

This Android application is written in Java and focuses on practical work with Bluetooth Low Energy (BLE). The project demonstrates a clear understanding of BLE architecture, Android permission handling, and structured application logic.

This module is part of a larger system currently under development and serves as a foundational component for BLE communication and device interaction.

What This Project Demonstrates
BLE Architecture Understanding

Knowledge of BLE roles and workflows, including advertising and scanning.

Correct use of core BLE components:

BluetoothAdapter

BluetoothLeAdvertiser

BluetoothLeScanner

Creation and parsing of BLE packets using:

Service UUIDs

Manufacturer-specific data

Handling real-world BLE constraints such as hardware support and device capabilities.

Android Permissions

Proper handling of runtime permissions required for BLE operations.

Detection of missing, denied, and permanently denied permissions.

Permission-aware application flow that prevents invalid operations.

Compatibility-conscious design aligned with Android system requirements.

Code Logic & Structure

Clear separation between UI actions and BLE logic.

Asynchronous programming using callbacks (ScanCallback, AdvertiseCallback).

Time-controlled scanning logic using handlers.

Defensive checks to avoid crashes and invalid states.

Consistent logging for debugging and validation.

Features

BLE Advertising with:

Custom Service UUID

Manufacturer-specific payload

Device name broadcasting

BLE Scanning for nearby devices

Extraction of:

Device name

RSSI (signal strength)

Advertised Service UUIDs

Manufacturer data

Runtime permission management

Time-limited scanning lifecycle

Technologies

Java

Android SDK

Bluetooth Low Energy (BLE)

Project Status

This project is actively under development and represents a functional subsystem within a broader application. Additional BLE functionality and system integration are planned as part of the larger project.

Notes

Requires a physical Android device with BLE support

Bluetooth must be enabled

Behavior may vary depending on hardware capabilities

Purpose

This project is intended to demonstrate practical understanding of BLE architecture, Android system APIs, permission management, and application-level logic.
