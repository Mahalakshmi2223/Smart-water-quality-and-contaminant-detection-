# AquaSense: Smart Water Quality & Contaminant Detection System

## Overview
This project monitors water quality in real-time and detects possible impurities or harmful substances.  
It uses multiple sensors to measure parameters like pH, turbidity, and dissolved solids (TDS).  
Based on sensor readings, the system can alert users if water is unsafe for consumption.

## Hardware Required
- Arduino Uno / NodeMCU (for IoT version)
- pH Sensor
- Turbidity Sensor
- TDS (Total Dissolved Solids) Sensor
- Buzzer or LED (for alert)
- Optional: LCD Display or IoT module (Blynk / Firebase) for live monitoring
- Jumper wires & breadboard

## Circuit Connections
- pH Sensor → Arduino Analog Pin A0  
- Turbidity Sensor → Analog Pin A1  
- TDS Sensor → Analog Pin A2  
- Buzzer → Digital Pin D8  
- GND & VCC as per sensor specifications

## How It Works
1. Sensors measure water parameters continuously.  
2. Threshold values are predefined for safe water:  
   - pH: 6.5 – 8.5  
   - Turbidity: < 5 NTU  
   - TDS: < 500 ppm  
3. If any parameter exceeds safe limits → alert via buzzer/LED.  
4. Optional IoT version → sensor data upload to mobile app / web dashboard for remote monitoring.

## Features
- Real-time water quality monitoring.  
- Easy to scale with IoT for remote monitoring.  
- Alerts for unsafe water automatically.  
- Can detect common contamination (impurities, excess dissolved solids, acidity/alkalinity).
