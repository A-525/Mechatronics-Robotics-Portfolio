# 🤖 Functional 3D-Printed WALL-E Robotic Replica (Raspberry Pi Architecture)

**Development Period:** October 2025  
**Author:** Andrés Santos Ibarra  
**Core Fields:** Additive Manufacturing, Multi-Actuator Robotics, Raspberry Pi Control  

---

## 📌 1. Project Overview
Mechatronic fabrication and control integration of a functional, articulated 3D-printed replica of the WALL-E robot, combining differential-drive mobile locomotion with multi-servo upper-body articulation.

---

## ⚙️ 2. Hardware & Mechatronic Specifications
* **Central Processing Unit:** Raspberry Pi single-board computer running Linux-based control scripts.
* **Articulated Upper Body (7-DOF):** 7 **SG90 micro-servomotors** controlling independent head pan/tilt, binocular eye inclination, and dual-arm/hand expressive movements.
* **Mobile Locomotion Base:** Tank-tread differential drive powered by **dual 100 RPM DC gear motors** via an H-Bridge motor driver.
* **Additive Manufacturing:** Multi-part PLA 3D-printed chassis, treads, and mechanical linkages sliced and optimized in UltiMaker Cura / Creality Print.

---

## 📂 3. Repository Contents
* `/control_scripts`: Python control scripts for Raspberry Pi GPIO / PWM servo sequencing and DC motor drive.
* `/media`: Assembly photos and actuation test videos.
