# LM3478 Boost Converter Hardware Design & Production

<img width="611" height="548" alt="image" src="https://github.com/user-attachments/assets/d2bd60f8-94d2-411d-bd27-98298420f916" />


## 📌 Project Overview
This project involves the complete hardware design, PCB layout, and physical prototyping of a boost (step-up) DC-DC converter using the Texas Instruments LM3478 High-Efficiency Low-Side N-Channel Controller. The primary goal of this project is to demonstrate end-to-end hardware engineering capabilities, from component selection and schematic capture to physical assembly and testing.

### ⚙️ System Specifications
* **Input Voltage (Vin):** 5V DC
* **Output Voltage (Vout):** 10V - 12V DC (Adjustable)
* **Maximum Output Current (Iout):** 2A
* **Switching Frequency (Fsw):** 200 kHz - 250 kHz

---

## 🛠️ Engineering Process & Hardware Implementation

### 1. Schematic & Component Selection
* Calculated inductor value to ensure Continuous Conduction Mode (CCM) operation at nominal loads.
* Selected a low-RDS(on) logic-level N-Channel MOSFET and a low forward-voltage Schottky diode to minimize switching and conduction losses.

### 2. PCB Layout Strategy
* Implemented a tight layout for the critical high di/dt output loop (MOSFET - Diode - Output Capacitor) to reduce parasitic inductance and ringing.
* Separated the power ground (PGND) and analog ground (AGND) to prevent switching noise from interfering with the LM3478's sensitive feedback and frequency compensation networks.

### 3. Manufacturing & Bring-up
* Generated industry-standard Gerber and NC Drill files.
* Hand-assembled the prototype board using SMD soldering techniques.
* Conducted functional testing to verify voltage regulation and stability under load.

---

## 📁 Repository Structure
* `\Hardware_Files`: Schematic and PCB Layout files.
* `\Manufacturing`: Gerber files, Drill files, and BOM (Bill of Materials).
