# Mechanical Module – 3 DOF Servo-Based Head

This directory contains the **mechanical design and implementation** of the **3-Degree of Freedom (3-DOF) servo-based head mechanism**, developed as part of the *IHuman-centric-home-assistant* project.

The mechanical system is designed to support smooth head movement and provide a physical platform for sensors such as a camera and display.

---

## Design Overview

The head mechanism provides **three degrees of freedom** to enable natural and expressive motion during interaction:

- **Yaw** – left and right rotation  
- **Pitch** – up and down movement  
- **Tilt / Nod** – forward and backward motion  

The structure is modular, compact, and suitable for 3D printing.

---

## Design & Fabrication

- **3D Modeling Tool:** Fusion 360  
- **Fabrication Method:** 3D Printing  
- **Actuation:** Servo Motors  
- **Material:** PLA (or equivalent)

All mechanical parts were designed to allow easy assembly and proper servo mounting.

---

## Servo-Based Head Movement

- Three-degree-of-freedom head movement for natural interaction  
- Smooth motion achieved using servo motors  
- Real-time motion control handled by a **dedicated microcontroller (ESP32)**  
- Offloads time-critical motion control from the main processor (Raspberry Pi)

---

## Current Status

### ✅ Completed
- 3D mechanical design completed in Fusion 360  
- Parts successfully 3D printed  
- Mechanical assembly of 3-DOF structure  
- Servo mounting and alignment
