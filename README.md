# 🚗 Smart Parking System with Satellite Communication

## 📌 Project Overview
This project implements a smart parking monitoring system using:

- Ultrasonic sensors
- Microcontroller
- EchoStar EM2050 satellite module
- MQTT broker
- Node-RED for data processing

The system detects vehicle entry and exit and transmits parking occupancy data via satellite.

---

## 🏗 Architecture

Ultrasonic Sensors → Microcontroller → EM2050 → Satellite → Gateway → MQTT → Node-RED

---

## 📊 Data Transmission

Payload is optimized using 3-byte hexadecimal encoding:

| Byte | Description |
|------|------------|
| 0    | Number of cars |
| 1    | Remaining spaces |
| 2    | Parking status (0=LIBRE, 1=DISPONIBLE, 2=PLEIN) |

---

## ⚙ Technologies Used

- C++ (Arduino)
- Satellite AT Commands
- MQTT
- Node-RED
- Base64 decoding

---

## 📸 Results

Real-time parking status successfully transmitted via satellite and decoded in Node-RED.

---

## 🚀 Future Improvements

- Web dashboard
- Mobile application
- Multi-parking support
- Energy optimization
