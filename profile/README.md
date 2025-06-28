# Advanced Driver Assistance System (ADAS) — Graduation Project

🚗 **Graduation Project – Department of Communications and Electronics Engineering**  
📅 Academic Year 2024–2025  
👩‍🏫 Supervised by: Dr. Aida El-Shafie

---

## 📌 Project Overview

This project aims to implement a real-time **Advanced Driver Assistance System (ADAS)** using embedded technologies. The system is designed to improve vehicle safety through intelligent features such as:

- 🛑 Automatic Emergency Braking (AEB)
- 🚘 Adaptive Cruise Control (ACC)
- 👀 Blind Spot Detection
- 🚧 Lane Detection
- 🚦 Traffic Sign Recognition
- 💤 Drowsiness Detection
- 📡 GPS Tracking and Dashboard GUI
- 📲 Firmware Over-The-Air (FOTA) updates

---

## 🧠 System Architecture

The solution is divided into two main subsystems:

### 🔹 STM32F103C8 (MCU)
- Runs a **custom RTOS**
- Implements real-time safety features:
  - Emergency braking
  - Blind spot detection
  - Adaptive cruise control
  - GPS data transmission
  - Motor control via PWM
- Communicates with Raspberry Pi via UART

### 🔹 Raspberry Pi 4 (Linux SBC)
- Runs a **custom Yocto-based Linux image**
- Performs vision-based tasks:
  - Lane detection (OpenCV)
  - Traffic sign recognition (YOLOv5)
  - GUI developed in Qt 6 (displaying speed, warnings, map, etc.)
- Supports **FOTA updates** for MCU firmware

---

## 📁 Repositories

| Module                    | Description                                  | Repository |
|---------------------------|----------------------------------------------|------------|
| `STM32`                  | Custom RTOS and embedded control logic       | [🔗 STM32 Repo](https://github.com/Graduation-Project-Automotive-ECE25/STM32) |
| `GUI`                    | Qt-based dashboard application               | [🔗 GUI Repo](https://github.com/Graduation-Project-Automotive-ECE25/GUI) |
| `ComputerVision`         | Lane & sign detection models/scripts         | *(Optional: add repo link)* |
| `Yocto-Image`            | Custom embedded Linux image for RPi          | [🔗 Yocto Repo](https://github.com/Graduation-Project-Automotive-ECE25/Yocto) |

---

## 🛠️ Key Technologies

- STM32F103C6T6 microcontroller
- Embedded C, FreeRTOS-like RTOS
- Raspberry Pi 4 with Yocto Linux
- Qt 6 for GUI (QML, Serial, WebEngine)
- OpenCV, YOLOv5
- Python, Bash
- UART Serial Communication
- GPS NEO-6M, HC-SR04, HC-05

---

## 📸 Screenshots

> _To be added_: GUI interface, lane detection demo, traffic sign inference, RTOS architecture diagram.

---

## 📚 Documentation

You can find the complete project documentation in the [`ADAS Graduation Book`](https://drive.google.com/file/d/1XIpy0AmPzTSJXAlBNidWxOked-inZP8N/view?usp=sharing)

---

## 👨‍💻 Contributors

Team Members:
- Assem Ayman (Team Leader)
- Mahmoud Walid
- Mahmoud Zayed
- Nada Metwaly
- Mohamed Ayman
- Ahmed Elbakr
- Hosam Ashraf
- Yomna Awny
- Omar Naeem

---

## 🔖 License

This project is licensed for academic use only.

