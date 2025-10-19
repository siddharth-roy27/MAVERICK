# 🛰️ MAVERICK – Modular Aerospace Embedded Flight Controller

**MAVERICK (Modular Aerospace Vehicle Embedded Real-time Intelligent Control Kit)** is a **dual-MCU flight control system** designed for **rockets, UAVs, and experimental aerospace platforms**.  
It combines **real-time control, telemetry, redundant sensors, and onboard intelligence** on a single PCB.

---

## 🖼️ Architecture Diagram

<img src="hardware/diagrams/MAVERICK Architecture.png" alt="MAEVRICK Architecture Diagram" width="700"/>

---

## 📖 Description

MAVERICK integrates the **STM32H7** main MCU for deterministic flight operations and an **ESP32-S3** companion MCU for telemetry, ML, and wireless communication.  
It provides **redundant sensor fusion**, **dual pyro channels**, **CAN networking**, and **modular expansion** for UAV and rocket platforms.

---

## ⚙️ Features

- **Dual MCU Architecture**: STM32H7 (real-time flight control) + ESP32-S3 (telemetry, ML, wireless)  
- **Redundant Sensing**: Dual IMUs (ICM-42688-P), ADXL375 high-g accelerometer, BMP388 barometer, Pitot sensor, u-blox GNSS  
- **Actuation & Safety**: 8 PWM servo outputs (PCA9685), dual pyro outputs (opto-isolated MOSFETs)  
- **Telemetry & Storage**: LoRa + Wi-Fi/BLE, microSD logging, CAN bus for inter-MCU and payload control  
- **Power Protection**: XT60 input, FET-switched servo rails, TVS diodes

---

## 🛰️ Applications

| Platform | Function |
|-----------|----------|
| 🚀 Rockets | Flight stabilization, stage ignition, recovery control |
| ✈️ UAVs / Drones | Autonomous flight, attitude stabilization, GPS navigation |
| 🧪 Aerospace Research | Sensor fusion, onboard ML, autonomous experiments |

---

## 🧩 Tech Stack

| Category | Components / Tools |
|----------|------------------|
| MCU | STM32H7, ESP32-S3 |
| Sensors | ICM-42688-P x2, ADXL375, BMP388, Pitot, u-blox GNSS |
| Communication | LoRa, Wi-Fi/BLE, CAN bus |
| Actuation | PCA9685 PWM, Pyro MOSFETs |
| Software | STM32CubeIDE, ESP-IDF, PlatformIO, KiCad 8 |
| Logging | microSD + GNSS PPS sync |
| Power | XT60 input, FET-switched rails, TVS protection |

---

## 🗂️ Repository Structure

MAVERICK/
├── LICENSE
├── README.md
├── .gitignore
├── BOM.csv
├── hardware/
│ ├── schematics/
│ ├── pcb/
│ ├── diagrams/
│ │ └── MAVERICK Architecture.png
│ └── README.md
├── firmware/
│ ├── stm32/
│ └── esp32/
├── docs/
│ ├── diagrams/
│ └── logs/
├── tools/
└── .github/
├── ISSUE_TEMPLATE.md
└── PULL_REQUEST_TEMPLATE.md

---

## 🌟 Vision

**MAVERICK** aims to **democratize aerospace flight control**, providing an **open, modular, and reliable platform** for makers, students, and researchers to develop rockets and UAVs with **autonomous flight and onboard intelligence**.

---

## 🔮 Future Scope

- Integration with **AI/ML flight path optimization**  
- **Multi-vehicle swarm communication** via CAN/LoRa  
- Support for **high-altitude telemetry and camera payloads**  
- Expansion to **hybrid rocket-UAV platforms** for advanced research  
- Development of **autonomous launch and recovery systems**
