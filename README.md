# 💧 Automatic Water Level Controller and Pump Automation System
 
A **hardware-based water level controller** designed to detect the current water level in a tank and automatically control the water pump.  
This system uses **transistors, operational amplifiers (Op-Amps), and metal contact sensors** no microcontroller is required.
 
---
 
## 🧠 Project Overview
 
The project automates water pump operation using simple analog components.  
It continuously monitors the water level inside a tank using **metal probe sensors**.  
When the water drops below a defined threshold, the circuit automatically turns the pump **ON**, and when the tank is full, it turns the pump **OFF**.
 
This design aims to **save water, electricity, and human effort** by providing a fully automatic solution with visual indication.
 
---
 
## ⚙️ Features
 
- 🌊 **Automatic Pump Control**  
  - Turns the motor **ON** when the tank is low.  
  - Turns the motor **OFF** when the tank is full.  
 
- 💡 **Water Level Indication**  
  - Uses **Red**, **Yellow**, and **Green LEDs** to represent **Low**, **Medium**, and **Full** levels respectively.  
 
- ⚡ **No Microcontroller Needed**  
  - Fully analog circuit based on **Op-Amps** and **Transistor switching**.
 
- 🔋 **Stable Power Supply**  
  - Includes a regulated dual power supply (+5V and -5V) using a **12V transformer**, **bridge rectifier**, **filter capacitor**, and **7805 regulator**.
 
- 🧩 **Reliable Design**  
  - Works with standard 220V AC input and 9V/12V DC pump systems.  
  - Compact, low-cost, and easy to assemble on PCB or breadboard.
 
---
 
## 🔌 Circuit Diagram
 
Below is the full hardware schematic used for the project:
 
![Circuit Diagram](https://github.com/galahal/Water-Level-Detector/blob/main/Hand%20drawn%20Circuit%20Diagram.png)
 
---
 
## 🧩 Components Used
 
| Component | Quantity | Description |
|------------|-----------|-------------|
| **220V–12V Transformer** | 1 | Steps down AC voltage |
| **Bridge Rectifier (Diodes)** | 4 | Converts AC to DC |
| **Voltage Regulator (7805)** | 1 | Provides +5V regulated output |
| **Capacitor (4.7µF)** | 1 | For DC smoothing |
| **Operational Amplifiers (Op-Amps)** | 4 | Used as comparators for level sensing |
| **Transistors (e.g., BC547)** | 3 | Drive LEDs based on water level |
| **LEDs (Red, Yellow, Green)** | 3 | Water level indicators |
| **Resistors (100Ω, 100kΩ, 2.2kΩ, etc.)** | — | For biasing and voltage division |
| **Metal Probes / Wires** | 4 | Water level contacts inside tank |
| **Relay + Pump (9V / 12V DC)** | 1 | Controls water flow |
| **Potentiometers (100kΩ)** | 3 | Adjustable voltage reference levels |
 
---
 
## 🧰 Power Supply Specification
 
- **Input:** 220V AC  
- **Step Down:** 12V AC via transformer  
- **Rectified Output:** +5V and -5V DC (for Op-Amp operation)  
- **Regulator:** 7805 provides stable +5V  
- **Reference:** -5V derived for comparator reference levels  
 
---
 
## ⚙️ Working Principle
 
1. **Metal contacts (M1–M4)** are placed at different heights inside the tank.  
2. The Op-Amps compare sensor voltages with predefined reference levels.  
3. Based on the comparator outputs:
   - **M1 (Low):** Pump turns ON, Red LED lights up.  
   - **M2/M3 (Medium):** Yellow LED turns ON.  
   - **M4 (Full):** Pump turns OFF, Green LED turns ON.  
4. The **relay driver circuit** controls the pump using a transistor as a switch.
 
---
 
## 🧪 How to Test
 
1. Connect the circuit as per the schematic.  
2. Use a **bucket or container** to simulate the water tank.  
3. Gradually increase the water level — watch the LEDs and motor response.  
4. Adjust **potentiometers** to fine-tune threshold levels.  
 
---
 
## 🧰 Tools & Equipment
 
- Breadboard / PCB board  
- Multimeter for testing  
- Soldering tools  
- 12V transformer  
- Small DC pump (9V or 12V)  
 
---
 
## 👨‍💻 Contributors
 
| Name | GitHub Profile |
|------|----------------|
| **Galahal** | [@Galahal](https://github.com/Galahal) |
| **Shreya Biswas** | [@Shreyaa-Biswas](https://github.com/Shreyaa-Biswas) |
 
---
 
🏫 *Course:* CSE251L — Digital Electronics Laboratory   
🔋 *Type:* Hardware-Based Analog Project (No Microcontroller)  
 
---
 
⭐ **If you found this helpful, consider giving the project a star on GitHub!**
