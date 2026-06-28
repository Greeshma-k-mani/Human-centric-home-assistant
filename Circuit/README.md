# PCB Design — EVA Human Centered Embodied Home Assistant

Circuit schematic and PCB layout for the EVA project, designed using **KiCad 9.0.5**.


---

## 📋 System Overview

| Controller | Role |
|------------|------|
| **Raspberry Pi 2 Model B** | Face recognition, voice interaction, navigation logic, Flask web UI |
| **ESP32 WROOM-32** | Motors, servos, TFT display, radar, HTTP server |
| **ESP8266 NodeMCU** | Garden relay control, WiFi automation |

---

## 🔌 Peripherals

| Component | Interface |
|-----------|-----------|
| ST7735R TFT Display | SPI |
| MG90S Servo × 3 (Yaw, Pitch, Roll) | PWM |
| TB6612FNG Motor Driver | PWM + GPIO |
| N25 Gear Motors × 2 | TB6612FNG |
| HLK-LD24 mmWave Radar | UART2 |
| 2-Channel Relay Module | GPIO (ESP8266) |
| PAM8403 Audio Amplifier | GPIO |

---

## ⚡ Power Architecture

- **Source:** 2S Li-ion Battery (7.4V)
- **MINI560:** 5V regulated — Raspberry Pi
- **Mini360:** 3.3V regulated — ESP32, ESP8266, logic
- **LM2590:** 6V regulated — Motors and servos
- **Protection:** 10A fuse + power switch
- **Decoupling:** Bulk and bypass capacitors on all power rails

---

## 📐 PCB Design Status

| Item | Status |
|------|--------|
| Schematic | ✅ Completed |
| PCB Layout | ✅ Completed |
| 3D Render | ✅ Completed |
| Fabrication | ✅ Fabricated |
| Testing | ✅ Tested |
| Design Tool | KiCad 9.0.5 |

---

---

## 📝 Design Notes

- Common ground reference across all modules
- Decoupling capacitors placed close to all ICs
- High-current motor and servo rails isolated from logic rails
- Designed for low-voltage, non-safety-critical academic use

---

> This PCB is part of an academic embedded systems project and is not intended for commercial or safety-critical applications.
