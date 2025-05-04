# FPV: Converting a 5" Racing Drone into an Autonomous Smart Platform

This project documents the conversion of a classic 5" racing FPV drone into an advanced, autonomous aerial platform using **ArduPilot** firmware and a **Raspberry Pi** companion computer.

## 🛠️ Current Hardware Setup

- **Frame**: 5" Mark4 copy
- **Flight Controller (FC)**: SpeedyBee F405 V3  
- **ESC**: 50A 4-in-1 BLHeli_S (included with FC)
- **Motors**: EMAX MT2204 II PLUS 2300KV ×4
- **Propellers**: iFlight 5"
- **Receiver**: HappyModel EP1 RX 2.4GHz (ELRS)
- **FPV Camera**: 9IMOD 1800TVL 5MP (OSD, Starlight Sensor)
- **VTX**: SpeedyBee TX800 (IRC Tramp compatible)
- **Antenna**: 80cm 5.8GHz
- **GPS**: HGLRC M100 (UART-based)
- **Companion Computer (Planned)**: Raspberry Pi 

## 🧠 Project Goals

- ✅ Build and test basic FPV functionality using Betaflight
- 🚧 Integrate GPS and enable telemetry
- 🔄 Flash and configure ArduPilot on SpeedyBee F405 V3 
- 🔌 Interface Raspberry Pi via MAVLink (UART)
- 🤖 Achieve basic autonomous functionality (Loiter, RTL, GPS hold)
- 📡 Enable real-time data logging, camera streaming, and Python-based mission scripting on RPi

## ⚙️ Planned Features

- MAVProxy or DroneKit integration on Raspberry Pi
- RPi-based logging and image processing
- Future upgrade to LiDAR or depth sensing
- Remote mission control via GCS (e.g., Mission Planner, QGroundControl)

## 🔧 Configuration Notes

- **FC Firmware**: `INAV` or `ArduPilot` (note: DShot not supported under INAV/ArduPilot for this board)
- **UART Assignments**:
  - UART1: Telemetry/MAVLink to RPi
  - UART2: Receiver (ELRS)
  - UART3: GPS (HGLRC M100)
  - UART4: VTX control (IRC Tramp)
  - UART5: ESC telemetry

- **Voltage Input**: 3–6S LiPo
- **BEC Outputs**: 5V 2A & 9V 2A (available for VTX, GPS, or RPi power via regulator)

## 📸 FPV System Specs

- Camera: 1800TVL 5MP, 1/8" starlight sensor, 2.1mm lens, WDR
- VTX: SpeedyBee TX800, 25–800mW, 40 channels, IRC Tramp protocol

## 🧪 Status

| Component        | Status           |
|------------------|------------------|
| Frame Build      | ✅ Complete       |
| Betaflight Setup | ✅ Complete       |
| GPS Integration  | 🔄 In Progress    |
| Ardupilot Setup  | ✅ Working on     |
| RPi Integration  | 🧠 Research Phase |
| ArduPilot Port   | 🧩 Testing        |

## 📚 Documentation

- [SpeedyBee F405 V3 Manual](docs/SpeedyBee_f405_v3_stack_manual_en.pdf)
- [TX800 VTX Manual](docs/TX800-manual_EN.pdf)
- [Camera Specs](docs/cameraSpec.txt)

## 🤝 Contributions

na
---

**Author**: Mateusz Cybruk 
**License**: na

