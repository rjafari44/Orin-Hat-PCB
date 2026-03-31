# Orin HAT Breakout Board

## Overview
The **Orin HAT** is a breakout board / HAT designed for the **NVIDIA Jetson AGX Orin**, providing smooth and organized pin connections for prototyping, development, and CAN bus tracing. This board simplifies access to GPIOs, communication buses, and power while ensuring robust protection for both the Jetson and connected peripherals.  

All signal lines on the HAT include **diodes for reverse current protection**, preventing accidental damage from reversed connections or miswiring.  

This PCB was designed using **Altium Designer** and was developed for **SC Robotics as a sub-project for the Mars Rover** to provide safe, reliable connections for rover development and testing.

---

## Features
- Breakout / HAT for **NVIDIA Jetson AGX Orin**  
- Dual voltage regulators:  
  - 12V → 3.3V  
  - 12V → 5V  
- IC buffers for clean, stable pin signals  
- **Every signal connection is protected by a diode** to prevent reverse current  
- CAN communication tracing support  
- Organized breakout pins for GPIO, power, and communication lines  
- Developed for **SC Robotics Mars Rover sub-project**  

---

## Components
- **Voltage regulators:** 12V → 3.3V, 12V → 5V  
- **IC buffers:** Protect Jetson pins and drive multiple outputs  
- **Diodes:** Reverse current protection on all signal lines  
- **Connectors:** Compatible with Jetson AGX Orin header  
- **Decoupling capacitors:** Stabilize voltage rails  
- **Breakout pins:** All Jetson GPIOs, power, and communication lines accessible  

---

## Wiring & Connections
| Connector / Pin | Function |
|-----------------|---------|
| 12V Input | Primary power supply for regulators |
| 3.3V Output | Powered by 12V → 3.3V regulator |
| 5V Output | Powered by 12V → 5V regulator |
| GPIO / Signal Lines | Buffered outputs connected to Jetson pins **through diodes for reverse current protection** |
| CAN_H / CAN_L | Traced and protected CAN communication lines |
| Ground (GND) | Common ground for Jetson and peripherals |

> **Note:** Every signal line passes through a diode, so reverse current from peripherals or miswiring is blocked. Always verify the 12V input is within tolerance.

---

## Usage
1. Mount the Orin HAT on the **NVIDIA Jetson AGX Orin** header.  
2. Connect a stable 12V power supply to the input.  
3. Connect peripherals or test circuits to the breakout pins. All signal lines are protected by diodes.  
4. Use the buffered GPIOs for clean signal driving and measurement.  
5. For CAN bus tracing, connect the CAN_H and CAN_L lines; the HAT protects the Jetson pins and allows reliable monitoring.  
6. Verify voltages at 3.3V and 5V outputs for any external devices if needed.  

---

## Applications
- Prototyping with **Jetson AGX Orin** GPIOs  
- CAN bus development and debugging  
- Sensor integration and robotics projects  
- Educational and research projects with Jetson platforms  
- Developed for **SC Robotics Mars Rover sub-project**  

---

## Images

### Schematic
![Schematic](assets/orin_hat_schematic.png)

### PCB Layout
![PCB Layout](assets/orin_hat_pcb_layout.png)

### 3D PCB Render
![3D PCB](assets/orin_hat_pcb_render.png)