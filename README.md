
# IoT-Based EV Battery Monitoring System with Cloud AI Health Prediction

An ESP32-based IoT prototype designed to monitor electric vehicle battery parameters and display battery information through local and cloud-connected interfaces.

## Project Overview

This project focuses on developing an IoT-based EV battery monitoring system using an ESP32 microcontroller. It monitors battery voltage, current, temperature, and flame-sensor information.

The system displays real-time measurements on a TFT touchscreen, provides battery information through a local HTTP/JSON interface, and uploads selected sensor data to ThingSpeak for remote monitoring through a React-based web dashboard.

## Main Features

- ESP32-based sensor acquisition and embedded processing
- Battery voltage and current monitoring
- DS18B20 temperature monitoring
- Flame-sensor input for safety-related monitoring
- ILI9341 TFT touchscreen display
- Embedded HTTP interface with `/api/battery` JSON endpoint
- ThingSpeak cloud data transmission
- React-based web dashboard
- Firmware-calculated battery indicators and nominal range estimate
- Relay, buzzer, and LED-based safety indications

## Hardware and Technologies

### Hardware Components
- ESP32 microcontroller
- Voltage sensor
- ACS712 current sensor
- DS18B20 temperature sensor
- Flame sensor
- ILI9341 TFT touchscreen
- XPT2046 touch controller
- Relay module
- Buzzer
- Indicator LEDs
- EV battery

### Software and Technologies
- Embedded C / Arduino IDE
- ESP32
- Wi-Fi communication
- HTTP and JSON
- ThingSpeak Cloud
- React.js
- CSS
- MATLAB (for research and analysis)

## System Architecture

The system follows this process:

1. Sensors collect battery parameters.
2. ESP32 processes the sensor readings.
3. Battery information is displayed on the TFT touchscreen.
4. Selected data is uploaded to ThingSpeak.
5. A React-based dashboard retrieves cloud data for remote visualization.

## Project Images

### 1. EV Battery Monitoring Hardware

![EV Battery Hardware](Images/project-hardware.jpg)

### 2. TFT Touchscreen Display

![TFT Display](Images/tft-display.jpg)

### 3. Web Dashboard

![Web Dashboard](Images/dashboard.jpg)

### 4. Sensor Connections

![Sensor Connections](Images/sensor-connections.jpg)

## Published Research Paper

**Title:** IoT-Based EV Battery Monitoring System with Cloud AI Health Prediction

**Journal:** International Journal of Scientific Research in Engineering and Management (IJSREM)

**Publication:** Volume 10, Issue 11, November 2026

**DOI:** 10.55041/IJSREM68809

**Authors:**
- Bhanuprakash K. R.
- Chandan S. G.
- Darshana K. A.
- Mrs. Amrutavarshini S. Hadimani

**Affiliation:** Department of Electronics and Communication Engineering, Kalpataru Institute of Technology, Tiptur, Karnataka, India.

[Read Published Research Paper (PDF)](Research-Paper/IJSREM-Research-Paper.pdf)

## Important Research Note

The implemented prototype calculates battery percentage, health-related indicators, remaining-life indication, and nominal range using programmed firmware logic.

The paper describes a cloud-based machine-learning framework as a proposed/future extension. It does not claim that a trained and experimentally validated AI model is integrated into the current prototype.

The calculated indicators are prototype estimates and should not be treated as validated battery state-of-health predictions or actual vehicle range.

## Repository Structure

```text
IoT-Based-EV-Battery-Monitoring-System/
│
├── Images/
│   ├── project-hardware.jpg
│   ├── tft-display.jpg
│   ├── dashboard.jpg
│   └── sensor-connections.jpg
│
├── Research-Paper/
│   └── IJSREM-Research-Paper.pdf
│
├── Project-Details/
│   └── project-overview.md
│
└── README.md
```

## Acknowledgement

Developed as an academic project in the Department of Electronics and Communication Engineering, Kalpataru Institute of Technology, Tiptur, Karnataka, India.
