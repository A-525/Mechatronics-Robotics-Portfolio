# 🕷️ Autonomous 8-DOF Quadruped Spider Robot with Neural Network Computer Vision

**Development Period:** March 2026 – June 2026  
**Author:** Andrés Santos Ibarra  
**Core Fields:** Mobile Robotics, Embedded Systems, Computer Vision, Neural Networks  

---

## 📌 1. Project Overview
Design, fabrication, and programming of an autonomous 8-Degrees-of-Freedom (8-DOF) quadruped walking robot capable of perceiving its environment through a trained Neural Network vision system and executing autonomous locomotion decisions (evading obstacles, sorting targets, or classifying geometric shapes and colors).

---

## 🔧 2. Hardware & Electromechanical Architecture
* **Main Microcontroller:** ESP32-S3 (Dual-core Xtensa LX7 with wireless communication and camera interface).
* **Kinematic Actuation (8-DOF):** 4 legs with 2 servomotors per leg (coxa/hip and femur/knee joints) driven via I2C communication by a **PCA9685 16-Channel 12-bit PWM Servo Driver**.
* **Proximity Sensing:** HC-SR04 Ultrasonic Sensor for real-time front obstacle distance measurement.
* **Chassis:** Custom 3D-printed PLA structural components designed for low weight and mechanical rigidity.

---

## 🧠 3. AI Vision Pipeline & Control Logic
1. **Image Acquisition & Preprocessing:** Real-time video stream processed in **Python (OpenCV)** for frame normalization, contour extraction, and color-space filtering.
2. **Neural Network Classification:** Custom-trained neural network model classifying geometric figures, specific color profiles, and predefined target objects.
3. **Closed-Loop Gait Execution:** The classification output is transmitted to the ESP32-S3 state machine, which triggers specific inverse-kinematic gait sequences:
   * **Avoidance Routine:** Dynamic turning maneuver when an obstacle or restricted marker is detected.
   * **Sorting / Action Routine:** Approaching and interacting with target objects based on class label.

---

## 📂 4. Repository Contents
* `/firmware_esp32`: C/C++ source code (PlatformIO / Arduino IDE) for servo PWM calibration and gait generation.
* `/vision_ai`: Python scripts, OpenCV processing pipeline, and trained neural network weights.
* `/media`: Demonstration videos and hardware assembly photographs.
