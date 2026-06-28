# EVA — Human Centered Embodied Home Assistant 🤖

> Voice-activated home assistant robot with face recognition, radar presence detection,
> expressive head movement, and smart home automation.
> 
> 🥇 **First Place — INNOVIX, RISE 2026 | FISAT ECE Department**

---

## 🧠 What is EVA?

EVA is a fully functional human-centric home assistant robot built on **Raspberry Pi 2 + ESP32**,
designed to recognize users, navigate to them, and assist through natural voice interaction.

Unlike conventional voice assistants, EVA physically moves to the user, verifies identity
through face recognition, and responds with expressive animations — making interaction
more natural and personal.

---

## ⚙️ System Architecture

```
┌─────────────────────────────────────────┐
│         RASPBERRY PI 2 MODEL B          │
│  Face Recognition · Voice · Navigation  │
│  Intent Engine · Flask Web UI · Groq AI │
└──────────────┬──────────────────────────┘
               │ HTTP (WiFi)
┌──────────────▼──────────────────────────┐
│              ESP32 WROOM-32             │
│  Motors · Servos · TFT · Radar · Face  │
└──────────────────────────────────────────┘
               │ HTTP (WiFi)
┌──────────────▼──────────────────────────┐
│            ESP8266 NodeMCU              │
│     Garden Relay · Light Control        │
└──────────────────────────────────────────┘
```

---

## 🔧 Features

| Feature | Details |
|---------|---------|
| 🎙️ Wake Word | Porcupine — "Hey Eva" |
| 👁️ Face Recognition | OpenCV — Haar + LBPH |
| 📡 Presence Detection | LD2410 mmWave Radar |
| 😊 Face Display | ST7735R TFT — 6 bitmap expressions |
| 🤖 3-DoF Head | MG90S servos — Yaw · Pitch · Roll |
| 🚗 Navigation | TB6612FNG + N25 gear motors |
| 🏠 Home Automation | ESP8266 relay — pump + lights |
| 🧠 AI Conversation | Groq LLM (Llama 3) |
| 🌐 Web UI | Flask dashboard — auth + controls |
| 🔌 Custom PCB | KiCad 9.0.5 — full system integration |
| 🖨️ Body | 3D printed enclosure (PLA) |

---

## 🛠️ Hardware

- Raspberry Pi 2 Model B
- ESP32 WROOM-32 DevKit
- ESP8266 NodeMCU
- Pi Camera Module V2 (NoIR)
- ST7735R TFT Display
- HLK-LD24 mmWave Radar
- TB6612FNG Motor Driver
- N25 Metal Gear Motors × 2
- MG90S Servo Motors × 3
- PAM8403 Audio Amplifier
- Custom PCB (KiCad 9.0.5)
- 2S Li-ion Battery (7.4V)

---

## 💻 Software Stack

```python
stack = {
    "Pi"      : ["Python 3", "OpenCV", "Porcupine", "Flask",
                 "edge-TTS", "Google STT", "Groq LLM"],
    "ESP32"   : ["Arduino C++", "WebServer", "SPI", "LEDC PWM"],
    "ESP8266" : ["Arduino C++", "ESP8266WebServer"],
    "PCB"     : ["KiCad 9.0.5"],
    "Body"    : ["Fusion 360", "3D Printing (PLA)"],
}
```

---


## 📬 Contact

[![GitHub](https://img.shields.io/badge/GitHub-Greeshma--k--mani-181717?style=for-the-badge&logo=github)](https://github.com/Greeshma-k-mani)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Greeshma%20K%20Mani-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/greeshma-k-mani)

---

GitHub: https://github.com/Greeshma-k-mani

LinkedIn: https://www.linkedin.com/in/greeshma-k-mani

<p align="center"><i>Built with curiosity. Powered by embedded silicon. Driven by the need to build things that actually work.</i></p>
