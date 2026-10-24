# 🔐 Cloud-Connected Biometric Automated Dispenser (Industry 4.0 & IoT)

**Development Period:** March 2026 – June 2026  
**Author:** Andrés Santos Ibarra  
**Core Fields:** Cyber-Physical Systems, Industrial IoT, Cloud Databases, Additive Manufacturing  

---

## 📌 1. Project Overview
Prototype of a smart, cloud-synchronized solid-candy dispensing machine demonstrating **Industry 4.0 mass-customization principles**. The system links optical biometric authentication directly to a cloud database to execute personalized multi-axis dispensing routines.

---

## ⚙️ 2. System Architecture & Workflow
1. **Biometric Authentication:** A user places their finger on the **AS608 Optical Fingerprint Sensor**. The **ESP32 microcontroller** captures and processes the biometric template ID.
2. **Real-Time Cloud Query (Google Firebase):** Via Wi-Fi, the ESP32 queries the **Firebase Realtime Database** to verify whether the fingerprint ID already has a registered dispensing configuration:
   * **Registered User Path:** The system retrieves the user's saved product combination and immediately activates the corresponding hopper servos and conveyor stepper motor.
   * **New User Path (HMI Configuration):** An interactive menu is displayed, allowing the user to select their desired solid products and quantities. The firmware translates this selection into motor step/angle parameters and saves the profile to Firebase linked to their fingerprint.
3. **Mechatronic Actuation:**
   * **Storage & Dosing:** Custom 3D-printed PLA hoppers actuated by servomotors.
   * **Transport System:** Linear conveyor belt driven by a **Nema 17 bipolar stepper motor** for precise product delivery.

---

## 🛠️ 3. Technologies Used
* **Hardware:** ESP32 Wi-Fi/BLE MCU, AS608 Fingerprint Module, Nema 17 Stepper Motor + Driver, SG90/MG995 Servomotors.
* **Cloud & Software:** Google Firebase Realtime Database, C/C++ (ESP32 Firmware), SolidWorks & UltiMaker Cura / Creality Print (3D CAD & Slicing).

---

## 📂 4. Repository Contents
* `/esp32_firebase_code`: Firmware source code for Wi-Fi connection, Firebase API integration, and AS608 sensor reading.
* `/cad_3d_models`: STL and SolidWorks files for the PLA hoppers and conveyor mounts.
* `/media`: System architecture diagrams and prototype demonstration photos/videos.
