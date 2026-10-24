# 🦾 Modeling, Simulation, and Robust-Adaptive Control of an Adept 600s SCARA Industrial Robot with Flexible Joints

**Project Type:** Undergraduate Engineering Thesis (Ongoing — Started Aug 2026)  
**Author:** Andrés Santos Ibarra  
**Institution:** Facultad de Ingeniería Mecánica y Eléctrica (FIME), UANL  

---

## 📌 1. Engineering Problem & Objective
High-speed industrial manipulators such as the **AdeptOne-XL / Cobra 600s SCARA robot** experience harmonic drive and transmission elasticity that induces residual mechanical vibrations, degrading end-effector positioning accuracy. 

The primary objective of this research is to formulate the complete non-linear mathematical model incorporating joint flexibility and design a **robust-adaptive control architecture** capable of:
* Suppressing elastic vibrations at the joints and end-effector.
* Ensuring high-precision trajectory tracking in the workspace.
* Compensating for parametric uncertainties and variable industrial payloads in real time.

---

## 🔬 2. Mathematical Modeling & Control Methodology
* **Kinematic Analysis:** Forward and inverse kinematics formulation using Denavit-Hartenberg (D-H) parameters for the 4-DOF SCARA configuration.
* **Dynamic Formulation (Euler-Lagrange):** Derivation of the coupled non-linear differential equations of motion modeling each elastic joint as a linear torsional spring connecting the actuator rotor and the rigid link:
  * Motor dynamics coupled with link inertia matrix $M(q)$, Coriolis/centripetal matrix $C(q, \dot{q})$, gravitational vector $G(q)$, and joint stiffness matrix $K$.
* **Control Strategy:** Robust-Adaptive Controller designed via Lyapunov stability theory to guarantee asymptotic tracking error convergence without requiring exact prior knowledge of payload mass or friction coefficients.

---

## 💻 3. Simulation & Software Environment
* **MATLAB / Simulink:** Numerical integration of the non-linear dynamic plant, adaptive law synthesis, and phase-plane stability analysis.
* **OpenModelica:** Multi-domain physical modeling and structural verification.
* **LaTeX / BibTeX:** Scientific documentation and mathematical typesetting.

---

## 📂 4. Repository Contents
* `/models`: MATLAB scripts (`.m`), Simulink block diagrams (`.slx`), and OpenModelica files.
* `/figures`: Trajectory tracking plots, joint torque profiles, and vibration damping curves.
* `/docs`: Mathematical derivation notes and thesis progress reports.
