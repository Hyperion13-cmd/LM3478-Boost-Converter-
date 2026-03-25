# LM3478 Boost Converter Hardware Design & Production

![LM3478 Physical Board]([BURAYA ÜRETTİĞİN KARTIN FOTOĞRAFINI VEYA 3D RENDER'INI EKLE])

## 📌 Project Overview
This project involves the complete hardware design, PCB layout, and physical prototyping of a boost (step-up) DC-DC converter using the Texas Instruments LM3478 High-Efficiency Low-Side N-Channel Controller. The primary goal of this project is to demonstrate end-to-end hardware engineering capabilities, from component selection and schematic capture to physical assembly and testing.

### ⚙️ System Specifications
* **Input Voltage (Vin):** [Örn: 5V - 12V]
* **Output Voltage (Vout):** [Örn: 24V]
* **Switching Frequency (Fsw):** [Örn: 400 kHz]
* **Max Output Current:** [Örn: 2A]

---

## 🛠️ Engineering Process & Hardware Implementation

### 1. Schematic & Component Selection
* Calculated inductor value to ensure Continuous Conduction Mode (CCM) operation at nominal loads.
* Selected a low-$R_{DS(on)}$ logic-level N-Channel MOSFET and a low forward-voltage Schottky diode to minimize switching and conduction losses.

### 2. PCB Layout Strategy
* Implemented a tight layout for the critical high $di/dt$ loop to reduce parasitic inductance and ringing.
* Separated the power ground (PGND) and analog ground (AGND) to prevent switching noise from interfering with the LM3478's sensitive feedback and frequency compensation networks.

### 3. Manufacturing & Bring-up
* Generated industry-standard Gerber and NC Drill files.
* Hand-assembled the prototype board using SMD soldering techniques.
* Conducted functional testing to verify voltage regulation and stability under load.

---

## 📁 Repository Structure
* `\Hardware_Files`: Schematic and PCB Layout files.
* `\Manufacturing`: Gerber files, Drill files, and BOM (Bill of Materials).
