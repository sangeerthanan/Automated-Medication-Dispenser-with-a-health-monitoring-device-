# Automated Medication Dispenser with a
 Health Monitoring Device  
This repository contains the code and documentation for a **Health Monitoring Device with a Smart Medibox**. The system integrates multiple sensors and actuators to monitor patient health, communicate data to a doctor, and manage a medication schedule with alerts and alarms.

## Features
- **Health Monitoring**: Collects patient data using temperature sensors and a MAX30102 sensor for heart rate and SpO2.
- **Remote Communication**: Sends health data to a doctor using Node-RED and MQTT protocol.
- **Automated Medication Dispenser**: Alerts the patient for medication with a buzzer, LEDs, and an alarm.
- **Storage Monitoring**: Maintains optimal temperature, humidity, and light conditions for medication.
- **Real-Time Clock (RTC)**: Ensures precise timing for alarms and notifications.
- **Alarm Button**: Allows manual configuration of alarms.

## Components Used
- **Microcontroller**: ESP32 WROOM Devkit (Onehorse ESP32 Dev Module)
- **Sensors**:
  - MAX30102 (heart rate and SpO2)
  - Temperature sensor
  - Humidity and light sensors
- **Actuators**:
  - Servo motor (for medibox compartments)
  - Buzzer
  - LEDs
- **OLED Display**: For displaying data
- **Connectivity**: MQTT protocol via Node-RED
- **Power Supply**: 9V battery

## System Architecture
1. **Data Collection**: Sensors collect health data.
2. **Data Transmission**: Sends collected data to the doctor via Node-RED.
3. **Decision Making**: Doctor sets the medication schedule remotely.
4. **Smart Medibox Alerts**:
   - Notifies the patient when to take medication.
   - Raises an alarm if storage conditions are not optimal.

## Requirements
### Hardware
- ESP32 WROOM Devkit
- Sensors: MAX30102, DHT11, and LDR
- Actuators: Servo motor, Buzzer, LEDs
- OLED Display
- Push button
- Power supply (e.g., 9V battery)

### Software
- Arduino IDE
- Node-RED
- MQTT Broker (e.g., Mosquitto)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/sangeerthanan/health-monitoring-device-with-a-smart-medibox.git
