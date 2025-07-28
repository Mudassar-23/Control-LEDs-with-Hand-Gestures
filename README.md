# 🔦 Control LEDs with Hand Gestures using MediaPipe, OpenCV & Arduino

Control real-world LEDs using just your hand gestures captured via webcam — no buttons, no touch!

## 🎯 Project Overview

This project demonstrates how to detect hand gestures using [MediaPipe](https://google.github.io/mediapipe/) and [OpenCV](https://opencv.org/) in Python, and control physical LEDs connected to an [Arduino](https://www.arduino.cc/) via serial communication.

Each finger movement is detected in real-time and mapped to control five LEDs, one for each finger.

---

## ⚙️ Tech Stack

- **Python**
- **OpenCV** – For webcam video capture and image processing
- **MediaPipe** – For real-time hand/finger tracking
- **Arduino UNO** – For receiving serial data and controlling LEDs
- **PySerial** – To communicate with Arduino via USB

---

## 📷 How It Works

1. The webcam captures a live video feed.
2. MediaPipe detects hand landmarks and analyzes finger positions.
3. A 5-element list is generated representing the state of each finger:
   * `1` → Finger is up  
   * `0` → Finger is down
4. This list is sent via serial communication to the Arduino.
5. The Arduino lights up LEDs based on the finger states.

---

## 🧰 Hardware Required

- Arduino Uno (or compatible board)
- 5 LEDs
- 5 Resistors (220Ω recommended)
- Breadboard and jumper wires
- USB cable for Arduino-PC connection

---

## 🖥️ Software Requirements

- Python 3.x
- OpenCV
- MediaPipe
- PySerial
- Arduino IDE

---
# Installation

## Hardware Setup:
- Connect each LED to Arduino pins 8–12 with a resistor in series.

## Arduino:

Upload the provided Arduino code using the Arduino IDE.
```bash
 https://www.arduino.cc/en/software/
```

## Python Environment:
```bash
pip install opencv-python 
pip install mediapipe
pip install pyserial
```
## Run the Python script:
```bash
 python main.py
```
#### Note:  Make sure to change COM8 to your correct Arduino COM port.
## 🧠 Applications

- Touchless control systems

- Gesture-based smart home interfaces

- Robotics hand control

- Educational demos in computer vision and embedded systems
