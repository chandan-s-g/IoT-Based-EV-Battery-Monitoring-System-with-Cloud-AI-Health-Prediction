# IoT-Based EV Battery Monitoring System

An ESP32-based prototype for monitoring electric-vehicle battery parameters and presenting selected information through local and cloud-connected interfaces.

## Project overview

The prototype collects battery voltage, current, temperature, and flame-sensor information using an ESP32. It presents measurements on a local TFT touchscreen, provides selected information through an embedded HTTP/JSON interface, and uploads configured measurements to ThingSpeak for remote visualization through a React-based dashboard.

## Main features

- ESP32-based sensor acquisition and embedded processing
- Battery voltage and current monitoring
- DS18B20 temperature monitoring
- Flame-sensor input for safety-related monitoring
- ILI9341 TFT touchscreen display
- Embedded HTTP interface with `/api/battery` JSON endpoint
- ThingSpeak cloud data transmission
- React-based web dashboard
- Firmware-calculated battery indicators and nominal range estimate

## Hardware and technologies

- ESP32 microcontroller
- Voltage sensor
- ACS712 current sensor
- DS18B20 temperature sensor
- Flame sensor
- ILI9341 TFT touchscreen and XPT2046 touch controller
- Relay, buzzer, and indicator LEDs
- Arduino/ESP32 embedded firmware
- Wi-Fi, HTTP, ThingSpeak, React, and CSS

## Research paper

The published paper is available here:

[`Research-Paper/IJSREM-Research-Paper.pdf`](Research-Paper/IJSREM-Research-Paper.pdf)

**Title:** IoT-Based EV Battery Monitoring System with Cloud AI Health Prediction  
**Journal:** International Journal of Scientific Research in Engineering and Management (IJSREM)  
**Issue:** Volume 10, Issue 11, November 2026  
**DOI:** 10.55041/IJSREM68809

**Authors:** Bhanuprakash K. R., Chandan S. G., Darshana K. A., and Mrs. Amrutavarshini S. Hadimani  
**Affiliation:** Department of Electronics and Communication Engineering, Kalpataru Institute of Technology, Tiptur, Karnataka, India.

## Important research note

The implemented prototype calculates battery percentage, health-related indicators, remaining-life indication, and nominal range using programmed firmware logic. The paper describes a cloud-based machine-learning framework as a proposed/future extension. It does not claim that a trained and experimentally validated AI model is integrated into the current prototype.

The calculated indicators are prototype estimates and should not be treated as validated battery state-of-health predictions or actual vehicle range.

## Repository contents

- `Research-Paper/` — published research paper PDF
- `Project-Details/` — additional project information

## Acknowledgement

Developed as an academic project in the Department of Electronics and Communication Engineering, Kalpataru Institute of Technology, Tiptur.
