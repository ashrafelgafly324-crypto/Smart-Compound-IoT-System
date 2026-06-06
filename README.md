# Smart Compound IoT Management System

## Overview
This repository contains the complete firmware and source code for the **Smart Compound System**, developed as an engineering graduation project. The system utilizes a distributed edge-computing architecture with multiple microcontrollers to manage access control, environmental safety, smart parking, and utility automation.

## System Architecture
The project is built upon a decentralized logic framework communicating via **ESP-NOW** for low-latency edge tasks, and synchronized globally using the **Arduino IoT Cloud** platform.

### Core Subsystems:
1. **VIP Security Node (ESP32-CAM & ESP8266):**
   - QR Code authentication using edge-vision processing.
   - Zero-latency actuation via ESP-NOW protocol.
   - Cloud synchronization for access logging.

2. **Intelligent Parking Management:**
   - Real-time IR sensor polling for 3D parking slot availability.
   - Dynamic pathway illumination using WS2811 addressable LEDs.
   - OLED visual routing and cloud override capabilities.

3. **Environmental Safety & Audio Alert:**
   - Distributed fire and smoke detection node.
   - Bluetooth A2DP audio streaming from SPIFFS for localized voice alarms.
   - Gateway node for remote dashboard notifications.

4. **Auxiliary Control & Smart Irrigation:**
   - LDR-based street lighting with software debounce logic.
   - Event-driven smart water pump automation via Arduino Cloud callbacks.

## Hardware Components
* ESP32-CAM AI-Thinker
* ESP32 & ESP8266 (NodeMCU)
* IR Sensors & Gas/Smoke Sensors
* Servo Motors & DC Water Pump
* OLED Display & WS2811 LED Strips

## Software & Libraries
* C/C++ (Arduino IDE)
* `ArduinoIoTCloud` & `Arduino_ConnectionHandler`
* `esp_now.h` & `WiFi.h`
* `FastLED`
* `ESP32QRCodeReader`
