<p align="center">
  <img src="images/logo.png" width="170" alt="EMOchi logo">
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="docs/README_FA.md">فارسی 🇮🇷</a>
</p>

<div align="center">

# 🤖 EMOchi

### An expressive Arduino OLED robot face

A lightweight emotional robot built with **Arduino Uno** and a **128×64 SSD1306 OLED** display. EMOchi combines animated eyes, blinking, emotions, sleep mode, and sensor interaction in a compact Arduino project.

<img src="images/demo.gif" width="600" alt="EMOchi demo">

![Arduino](https://img.shields.io/badge/Arduino-Uno-00979D?style=for-the-badge&logo=arduino)
![OLED](https://img.shields.io/badge/OLED-SSD1306-blue?style=for-the-badge)
![Language](https://img.shields.io/badge/C%2B%2B-Arduino-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</div>

---

## ✨ Features

- 👀 Smooth animated robot eyes
- 😉 Automatic blinking
- 👈👉 Idle eye movement
- 😊 Happy expression
- 😠 Angry expression
- 🌙 Automatic sleep mode
- ☀️ Wake-up behavior based on light
- 👆 Touch interaction
- 💡 LDR light detection
- ⚡ Designed for Arduino Uno
- 🧠 Lightweight animation logic

---

## 🧩 Hardware

| Component | Quantity |
|---|---:|
| Arduino Uno | 1 |
| SSD1306 OLED 128×64 I2C | 1 |
| Touch Sensor | 1 |
| LDR Module | 1 |
| Jumper Wires | Several |

---

## 🔌 OLED Wiring

| OLED | Arduino Uno |
|---|---|
| VCC | 5V |
| GND | GND |
| SDA | A4 |
| SCL | A5 |

> **Note:** Sensor pin assignments are defined by the Arduino sketch. Check the source code before wiring the Touch Sensor and LDR module.

---

## 📦 Requirements

### Hardware

- Arduino Uno
- 128×64 SSD1306 OLED with I2C
- Touch sensor
- LDR module

### Arduino Libraries

Install these libraries through the Arduino IDE Library Manager when required by the sketch:

- **Adafruit GFX Library**
- **Adafruit SSD1306**
- **FluxGarage RoboEyes** — only if your sketch uses the external library version rather than the bundled RoboEyes implementation

> **Important:** The current repository contains RoboEyes implementation code inside `Arduino_Code/OLED_Emotion_Robot.ino`. The project should not include a second conflicting RoboEyes implementation when compiling.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/hadipashaw/EMOchi.git
cd EMOchi
```

### 2. Open the Arduino project

Open the Arduino sketch from:

```text
Arduino_Code/OLED_Emotion_Robot.ino
```

### 3. Install the required libraries

Install the libraries required by the sketch from the Arduino IDE Library Manager.

### 4. Select the board

In Arduino IDE, select:

```text
Board: Arduino Uno
```

### 5. Connect the hardware

Wire the OLED and sensors according to the wiring section and the pin definitions in the sketch.

### 6. Compile and upload

Connect the Arduino Uno through USB, compile the sketch, and upload it to the board.

---

## 🎮 Behavior

| Input / Event | Behavior |
|---|---|
| Power On | Starts the robot animation |
| Idle timer | Eyes move to different positions |
| Automatic timer | Eyes blink randomly |
| Touch | Triggers an interactive emotion |
| Darkness | Enters sleep behavior |
| Light returns | Wakes from sleep behavior |

The exact timing and sensor behavior are controlled by the values in the Arduino sketch.

---

## 📁 Project Structure

```text
EMOchi/
├── Arduino_Code/
│   └── OLED_Emotion_Robot.ino
├── docs/
│   └── README_FA.md
├── images/
│   ├── demo.gif
│   ├── logo.png
│   └── robot.jpg
├── LICENSE
└── README.md
```

---

## 📸 Gallery

<p align="center">
  <img src="images/robot.jpg" width="450" alt="EMOchi robot">
</p>

---

## 🙏 Credits

EMOchi is inspired by the open-source Arduino and OLED community.

Special thanks to:

- [FluxGarage RoboEyes](https://github.com/FluxGarage/RoboEyes)
- [Adafruit](https://github.com/adafruit)

---

## 📜 License

This project is licensed under the **MIT License**.

See [LICENSE](LICENSE) for the complete license text.

---

<div align="center">

⭐ If you find EMOchi useful, consider giving the repository a star.

</div>
