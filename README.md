# Investigation Influences of Pulling Speed on Stripe Pattern Formation of Peeled Tape

 **National Chung Cheng University | Final Project for Experiments on Fundamental Physics 2B | 2026 Joint Physics Education Meeting of ROC**

This project explores the underlying physical mechanisms of the everyday phenomenon of "peeling transparent tape." It features not only experimental data and mechanical analysis but also a web-based **interactive physics simulator** to visualize the dynamic behavior of polymer adhesives under varying peeling speeds.

---

##  Introduction

When peeling off transparent tape, the peeled surface often exhibits alternating "White Zones" and "Transparent Zones". Variations in peeling speed directly affect the peeling resistance, the pitch of the sound produced, and the spatial distribution of these stripes. This study aims to establish an experimental system capable of stably and quantitatively controlling the pulling speed to investigate:
1. The influence of pulling speed on critical peeling force and dynamic tension variations.
2. The evolutionary patterns of the stripe characteristics (White/Transparent Zone width) on the tape at different pulling speeds through quantitative analysis.

##  Physics Theory

This study explains the **Stick-Slip Instability** through macroscopic dynamics and microscopic polymer physics:

*   **Macroscopic Dynamics: Spring-Block Model**
    $$m\ddot{x}=k(vt-x)-F(\dot{x})$$
    The tape substrate is modeled as a spring, and the peeling junction as a block. The system periodically alternates between accumulating elastic potential energy (Stick) and sudden sliding (Slip).
*   **Microscopic Mechanism: Deborah Number ($De$)**
    *   **Low-speed regime ($De \ll 1$)**: The polymer chains have sufficient time to relax, remaining in a "rubbery state", which causes macroscopic drawing (fibrillation) and forms the White Zone.
    *   **High-speed regime ($De \gg 1$)**: The peeling time is extremely short, forcing the adhesive into a "glassy state". This results in brittle fracture, leaving a flat, transparent surface. Meanwhile, the "viscoelastic stiffening" effect causes the peeling resistance to rise as speed increases.

## 🛠️ Experimental Setup

We designed and constructed a **Three-Pulley Traction System**:
*   **Motion Control**: Utilizing a microcontroller and a stepper motor to precisely control the peeling speed of the tape.
*   **Tension Measurement**: Integrated with a force sensor to capture micro-dynamic tension variations (F-t curves) in real-time during the peeling process.
*   **Stabilization Mechanism**: A combination of one movable pulley and two fixed pulleys ensures uniform force distribution and stable traction direction.

## 📊 Key Findings

1.  **Three Dynamic Regimes**: The relationship between pulling speed and peeling force can be divided into a "Very Slow Regime (steady)", an "Unstable Regime (violent oscillations)", and a "Fast Regime (rising force)".
2.  **Stripe Spacing Rules ($\lambda = \lambda_{stick} + \lambda_{slip}$)**:
    *   **White stripe ($\lambda_{stick}$)** decreases as pulling speed increases.
    *   **Transparent stripe ($\lambda_{slip}$)** increases as pulling speed increases.
    *   **Total stripe spacing ($\lambda$)** decreases as pulling speed increases, verifying the daily observation that "the faster you peel the tape, the denser the residual stripes become."

## Interactive Simulator

This project includes a built-in web simulator to demonstrate the experimental results, allowing users to:
*   **Adjust the Pulling Speed**
*   **Observe the tension-time (F-t) waveform variations in real-time**
*   **Visualize the evolution of the stripe patterns on the tape**

> **Usage**: Simply open `index.html` in your browser and switch to the "7. 互動模擬器 (Interactive Simulator)" tab, or open `simulator.html` directly to experience it.

##  Team

*   **Authors**: Zheng-Da Tsai, Chang-Yu Wu (Web Developer), and Zhung-Rui Zhang.
*   **Advisor**: Prof. Pi-Hui Tuan
*   **Institution / Event**: National Chung Cheng University / 2026 Joint Physics Education Meeting of ROC (Undergraduate Group).

##  References

1. Grzelka, M., et al. (2022). *Transition from viscoelastic to fracture-like peeling of pressure-sensitive adhesives.* Soft Matter.
2. Everaerts, A. I., & Clemens, L. M. (2002). *Chapter 11 - Pressure sensitive adhesives.* Adhesion Science and Engineering.

---
*© 2026 Chang-Yu Wu, Zheng-Da Tsai, and Zhung-Rui Zhang. All rights reserved.*
