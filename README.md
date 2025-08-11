we aimed to help the elderly to overcome fear and prevent falling .we initially aimed to increase accuracy by implementing ai model through tensorflow lite but we faced challenges while training data and running the model in esp32 so due to time and knowledge constraints we focused on   calibrating  our sensor to detect fall motion with mpu6050 and hooking it with esp32 we used blynk to make an iot output where messages and alerts are notified
# ESP32 Fall Detection System

## 📌 Overview
This project implements a **Fall Detection System** using an **ESP32** and **MPU6050** accelerometer & gyroscope sensor.  
The system detects sudden changes in acceleration/angle that indicate a fall, then triggers an **alert** via buzzer, OLED display, and/or network notification.

**Features:**
- Detects falls in real-time using motion data
- Configurable sensitivity threshold
- Buzzer alert on fall detection
- Optional OLED message display (`Fall Detected!`)
- Optional Wi-Fi alert (Blynk / HTTP / MQTT)

---

## 🛠 Hardware Required
| Component           | Quantity |
|---------------------|----------|
| ESP32 Dev Board     | 1        |
| MPU6050 Sensor      | 1        |
| Buzzer (Piezo)      | 1        |
| 0.96" OLED Display  | 1 *(optional)* |
| Jumper Wires        | As needed |
| Breadboard          | 1        |

---

## 📡 Connections

### MPU6050 → ESP32
| MPU6050 Pin | ESP32 Pin |
|-------------|-----------|
| VCC         | 3.3V      |
| GND         | GND       |
| SCL         | GPIO 22   |
| SDA         | GPIO 21   |



---
