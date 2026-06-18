# 🚜 Vehicle Monitoring System J1939

CANBUS J1939 Vehicle Monitoring System using MQTT, Python, InfluxDB, Grafana, Telegram Alert and Daily Email Report

-

## Overview

This project was built to learn CANBUS SAE J1939 and basic telematics systems.

Saya mulai dari belajar konsep PGN, SPN, Start Bit, Length, Scaling Factor, Offset, dan Little Endian pada CANBUS J1939. Setelah memahami proses decoding data CANBUS, saya membuat simulasi vehicle monitoring system menggunakan ESP32, MCP2515, MQTT, Python, InfluxDB, Grafana, Telegram Alert, dan Daily Email Report.
Data RPM, Temperature, dan Fuel disimulasikan menggunakan 3 potentiometer. Data tersebut dikirim melalui MQTT, diproses menggunakan Python, disimpan ke InfluxDB, kemudian ditampilkan pada Grafana Dashboard secara real-time.

Project ini berfokus pada pemahaman proses decoding CANBUS J1939 serta implementasi alur data telematics sederhana mulai dari data acquisition, processing, storage, visualization, hingga alert notification.
---

## Features

- CANBUS J1939 PGN/SPN Decoding
- ESP32 Sender & Receiver Communication
- MQTT Data Transmission
- Python MQTT Subscriber
- InfluxDB Data Storage
- Grafana Real-Time Dashboard
- RPM, Temperature and Fuel Monitoring
- Telegram Alert Notification
- Daily Email Report
- CANBUS Message Investigation & Validation

---

## Learning Journey

- CANBUS Loopback Testing
Started with MCP2515 loopback mode to understand basic CAN communication.

- Sender and Receiver Communication
Built a simple CAN sender and receiver using ESP32 and MCP2515 modules.

- CAN Message Analysis
Captured and analyzed CAN frames to understand message structure.

- DBC Decoding Practice
Learned PGN, SPN, start bit, signal length, scaling factor and offset.

- Vehicle Monitoring System
Integrated MQTT, Python vscode, InfluxDB, Grafana, Telegram alerts and Daily Report into a simple telematics simulation.

---

## System Architecture

![Architecture](Architectur_canbus.png)

---

## Technologies

- ESP32
- MCP2515 CANBUS Module
- Arduino IDE
- CANBUS SAE J1939
- MQTT
- MQTTX
- EMQX Broker
- Python
- VS Code
- InfluxDB
- Grafana
- Telegram Bot
- SMTP Email

---

## J1939 Signals Used

- PGN 61444 - SPN 190 (Engine RPM)
- PGN 65262 - SPN 110 (Coolant Temperature)
- PGN 65262 - SPN 174 (Fuel Temperature)
- PGN 65262 - SPN 175 (Oil Temperature)
- PGN 65271 - SPN 158 (Battery Voltage)
- PGN 65253 - SPN 236 (Engine Hours)
  
Topics learned:

- PGN
- SPN
- Start Bit
- Length
- Endianness
- Scaling Factor
- Offset
- Raw CAN Decoding

---

## Dashboard

Dashboard displays:

![Dashboard](Dashboard_vehicle_data)

---

## Future Improvements

- Real CANBUS Interface
- GPS Tracking
- Fleet Monitoring
- Maintenance Analytics
- Heavy Equipment Telematics

---

## Author
Marwan Saputra

Self-learning CANBUS SAE J1939, MQTT and Telematics Systems.


## Hardware Setup

![Hardware](hardware.png)

## MQTT Architecture

![MQTT](mqtt.png)

## Node-RED Flow

![NodeRED](node-red.png)

## Real Time Dashboard

![Dashboard](dashboard_realtime.png)

## Historical Data

![History](table.history.png)

## Telegram Alert

![Alert](alert.png)


## Demo Videos

### Demo 1 - CAN Bus J1939 Decoding

A short demonstration of how I decode J1939 CAN messages and convert raw data into engineering values.

https://drive.google.com/file/d/1FIqOyyu8uFpCbvV_N2UNnbVg5x24gt2q/view?usp=drivesdk

### Demo 2 - End-to-End Vehicle Monitoring System

A complete demonstration of the project from CAN Bus simulation to dashboard monitoring and Telegram alerts.

https://drive.google.com/file/d/1CyV-6kXFwHmTgpQlI_nw35109WbvViyo/view?usp=drivesdk
