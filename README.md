This project is licensed under the [Apache License 2.0](LICENSE).  
© 2025 Mateusz.


# FPV: Converting a 5" Racing Drone into an Autonomous Smart Platform

This project documents the conversion of a classic 5" racing FPV drone into an advanced, autonomous aerial platform using **BetaFlight** firmware and a **Raspberry Pi** companion computer.

## Current Hardware Setup

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
- **Companion Computer**: Raspberry Pi 
- **Computer vison camera**: Raspberry Pi Camera Module 3

## Project Goals

-  Build and test basic FPV functionality using Betaflight ✅
-  Integrate GPS and enable telemetry ✅
-  Flash and configure BetaFlight on SpeedyBee F405 V3 ✅
-  Interface Raspberry Pi via MAVLink (UART)
-  Interface Raspberry Pi via MSP ✅
-  Achieve basic autonomous functionality (Loiter, RTL, GPS hold) ✅
-  Enable real-time data logging, camera streaming, and Python-based mission scripting on RPi
-  Enable GPS-denied navigation
-  Enable fully autonomous flight
-  Enable object detection
-  Enable object avoidance via Computer Vision and Lidar


## Configuration Notes

- **FC Firmware**: BetaFlight
- **UART Assignments**:
  - UART1: 
  - UART2: Receiver (ELRS)
  - UART3: GPS (HGLRC M100)
  - UART4: VTX control (IRC Tramp)
  - UART5: ESC telemetry
  - Usb C - Raspbery Pi usb



## FPV System Specs

- Camera: 1800TVL 5MP, 1/8" starlight sensor, 2.1mm lens, WDR
- VTX: SpeedyBee TX800, 25–800mW, 40 channels, IRC Tramp protocol
- Raspberry Pi Camera Module 3 (computer vision)


## Documentation

- [SpeedyBee F405 V3 Manual](docs/SpeedyBee_f405_v3_stack_manual_en.pdf)
- [TX800 VTX Manual](docs/TX800-manual_EN.pdf)
- [Camera Specs](docs/cameraSpec.txt)

## 🤝 Contributions

na
---

**Author**: Mateusz Cybruk 
**License**: Apache 2.0 

