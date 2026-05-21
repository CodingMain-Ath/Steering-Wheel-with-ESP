# 🎮 ESP32 Wireless Steering Wheel Controller

> A wireless steering wheel controller built on ESP32 with real-time telemetry over Wi-Fi.

[![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)](https://www.espressif.com/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)]()

**Live Demo:** [steering-wheel-with-esp.vercel.app](https://steering-wheel-with-esp.vercel.app)

---

## 📌 Overview

This project turns an ESP32 into a wireless steering wheel controller. Sensor data from the ESP32 is streamed in real-time to a web-based dashboard via WebSocket, giving live feedback on steering angle, throttle, and system state.

## ✨ Features

- **Wireless control** — ESP32 hosts a Wi-Fi access point for direct connection
- **Real-time telemetry** — Live data streamed via WebSocket to browser dashboard
- **Web UI** — Clean, mobile-friendly control interface
- **Low latency** — Sub-20ms round-trip response time
- **Plug and play** — No app install needed, runs in any browser

## 🛠️ Hardware

| Component | Part |
|---|---|
| MCU | ESP32 DevKit V1 |
| Sensor | MPU-6050 (tilt-based steering) |
| Power | 3.7V LiPo |

## 🚀 Getting Started

```bash
git clone https://github.com/CodingMain-Ath/Steering-Wheel-with-ESP.git
cd Steering-Wheel-with-ESP
# Flash firmware to ESP32 via PlatformIO
# Connect your phone/PC to the ESP32 Wi-Fi hotspot
# Open the dashboard URL in a browser
```

## 🏗️ Architecture

```
ESP32 (Access Point + WebSocket Server)
      │
      │── Wi-Fi ──▶ Browser (Web Dashboard)
      │                   │
      ▼                   ▼
Sensor Reading        Live Telemetry Display
```

## 📄 License
MIT © Atharv Huilgol
