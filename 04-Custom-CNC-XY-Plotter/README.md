# 📐 Design and Fabrication of a Custom 2-Axis CNC XY Plotter Machine

**Development Period:** January 2025 – June 2025  
**Author:** Andrés Santos Ibarra  
**Core Fields:** CNC Automation, CAD/CAM, Motion Control, Mechatronic Design  

---

## 📌 1. Project Overview
Complete design, mechanical assembly, electronic wiring, and G-Code configuration of a custom 2-Axis (X-Y) Computer Numerical Control (CNC) drawing plotter capable of executing complex 2D vector trajectories with a precision pen end-effector.

---

## 🛠️ 2. Mechanical & Electronic Engineering
* **Structural & Linear Motion System:**
  * X and Y linear motion axes built using precision linear guide rods, linear ball bearings, timing belts/lead screws, and custom 3D-printed PLA structural brackets.
  * Z-axis actuated pen-holder mechanism for automated pen-up / pen-down transitions between drawing paths.
* **Drive & Control Electronics:**
  * Bipolar stepper motors paired with microstepping current drivers for smooth velocity profiling and minimal resonance.
  * Microcontroller running CNC motion-control firmware with hardware limit switches (end-stops) for automated homing cycles.

---

## 💻 3. CAD/CAM to G-Code Pipeline
1. **Vector Design:** Creation and scaling of 2D technical drawings and geometric patterns.
2. **CAM Toolpath Generation:** Conversion of vector paths into standardized **G-Code** (`G00` rapid positioning, `G01` linear interpolation, `G02/G03` circular interpolation) with calibrated feed rates ($F$) and workspace coordinates.
3. **Trajectory Execution:** Serial streaming of G-Code commands to the microcontroller for synchronized dual-axis interpolation.

---

## 📂 4. Repository Contents
* `/gcode_samples`: Test G-Code routines and calibration patterns.
* `/cad_mounts`: 3D CAD models of the mechanical couplings and pen-holder assembly.
* `/media`: Videos and photographs of the CNC machine plotting in real time.
