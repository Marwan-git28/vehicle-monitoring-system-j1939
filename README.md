# 🚜 Vehicle Monitoring System J1939

CANBUS J1939 Vehicle Monitoring System using MQTT, Node-RED, SQLite and Telegram Alert.

---

## Overview

This project demonstrates a real-time vehicle monitoring system inspired by telematics applications used in heavy equipment and fleet monitoring.

Telemetry data is simulated using Arduino and potentiometers, transmitted via MQTT, processed by Node-RED, stored in SQLite, displayed on a real-time dashboard, and integrated with Telegram notifications.

---

## Features

- Real-Time Monitoring Dashboard
- MQTT Communication
- SQLite Data Logging
- History Monitoring (10 Minutes, 1 Hour, 1 Day)
- Alert History (10 Minutes, 1 Hour, 1 Day)
- Telegram Alert Notification
- CANBUS J1939 Decoding Study

---

## System Architecture

Arduino + Potentiometers
↓
MQTT Publisher
↓
EMQX Broker
↓
Node-RED
├── Dashboard
├── SQLite Database
└── Telegram Alert
↓
End User

---

## Technologies

- Arduino
- MQTT
- MQTTX
- EMQX
- Node-RED
- SQLite
- Telegram Bot
- CANBUS SAE J1939

---

## J1939 Knowledge Applied

### PGN 61444

SPN 190 - Engine RPM

### PGN 65262

SPN 110 - Coolant Temperature

SPN 174 - Fuel Temperature

SPN 175 - Oil Temperature

### PGN 65271

SPN 158 - Battery Voltage

### PGN 65253

SPN 236 - Engine Hours

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

- RPM
- Temperature
- Fuel
- Historical Data
- Alert History
- Real-Time Monitoring

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

Self-learning CANBUS J1939 and Telematics Enthusiast.
