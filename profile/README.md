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

## 🎥 Demonstrations

> Click the images below to watch full demonstrations.

| Feature | Preview | Description |
|--------|---------|-------------|
| **Intro Video** | [![Intro](videos/thumbnails/intro.png)](videos/intro.mp4) | Full system overview |
| **Adaptive Cruise Control** | [![ACC](https://github.com/Graduation-Project-Automotive-ECE25/.github/blob/main/videos/thumbnails/Acc.jpg)](https://github.com/Graduation-Project-Automotive-ECE25/.github/blob/main/videos/ACC.mp4) | Adjusts speed based on front vehicle |
| **Automatic Emergency Braking** | [![AEB](videos/thumbnails/aeb.png)](videos/aeb.mp4) | Stops automatically if an object is detected |
| **Blind Spot Detection** | [![Blind Spot](videos/thumbnails/blindspot.png)](videos/blindspot.mp4) | Warns driver of vehicles in blind spots |
| **GPS Tracking** | [![GPS](videos/thumbnails/gps.png)](videos/gps.mp4) | Displays vehicle location on the map |
| **Lane Departure Warning** | [![Lane](videos/thumbnails/lane.png)](videos/lane.mp4) | Alerts when lane deviation is detected |
| **Traffic Sign Detection** | [![Signs](videos/thumbnails/signs.png)](videos/signs.mp4) | Recognizes and classifies traffic signs |
| **Overspeed Warning** | [![Speed](videos/thumbnails/overspeed.png)](videos/overspeed.mp4) | Issues GUI warning on speed limit breach |
| **Yocto Boot** | [![Yocto](videos/thumbnails/yocto.png)](videos/yocto.mp4) | Custom embedded Linux startup and GUI |
| **Firmware OTA** | [![FOTA](videos/thumbnails/fota.png)](videos/fota.mp4) | Demonstrates remote firmware update |


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

