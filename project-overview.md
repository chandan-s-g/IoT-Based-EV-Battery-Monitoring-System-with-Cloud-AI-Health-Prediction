# Project Overview

## Objective
Develop an ESP32-based prototype that monitors selected EV battery parameters and makes the measurements available locally and remotely.

## Monitoring inputs
- Battery voltage
- Battery current (ACS712)
- Battery temperature (DS18B20)
- Flame-sensor status

## Processing and interfaces
The ESP32 processes sensor inputs, updates the ILI9341 TFT touchscreen, provides selected data through a local HTTP JSON endpoint, and transmits configured fields to ThingSpeak. A React-based dashboard retrieves the latest cloud feed for remote visualization.

## Scope and limitations
Battery percentage, health-related indicators, remaining-life indication, and nominal range are calculated using programmed firmware logic. The paper proposes a cloud machine-learning framework for future battery-health analysis; a trained and experimentally validated AI model is not claimed as part of the current prototype.

See the published paper in `../Research-Paper/IJSREM-Research-Paper.pdf` for the full methodology, architecture, and evaluation.
