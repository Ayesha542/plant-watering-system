# Automatic Plant Watering System

## Overview
An automated irrigation system that monitors soil moisture levels and waters plants automatically when the soil becomes too dry, removing the need for manual watering and helping prevent both overwatering and underwatering.

## Features
- Real-time soil moisture monitoring
- Automatic water pump activation based on moisture threshold
- LED/Serial monitor indication of soil status (dry/wet)
- Adjustable moisture threshold in code
- Low-cost and easily expandable to multiple plants

## Components Used
- Arduino Uno
- Soil moisture sensor
- 5V mini submersible water pump
- Relay module (to switch pump on/off)
- Water reservoir and tubing
- Jumper wires, breadboard
- Power supply

## How It Works
1. The soil moisture sensor is inserted into the soil and continuously reads moisture levels.
2. The Arduino compares the reading against a defined dryness threshold.
3. If soil moisture falls below the threshold, the Arduino triggers the relay to activate the water pump.
4. The pump draws water from the reservoir and irrigates the soil.
5. Once the moisture level rises above the threshold, the pump automatically switches off.

## Circuit Diagram
*(Insert circuit diagram image here — e.g., `circuit-diagram.png`)*

## Code
See `plant_watering.ino` for the Arduino sketch containing sensor reading logic, threshold configuration, and pump control.

## Setup & Testing
1. Insert the soil moisture sensor into the target plant's soil.
2. Connect the relay module to control the water pump, with the pump tubing placed in the reservoir and directed to the soil.
3. Upload `plant_watering.ino` to the Arduino.
4. Test by allowing soil to dry out and observing automatic pump activation, then confirm it switches off once soil is adequately moist.
5. Calibrate the moisture threshold value in code based on your specific sensor and soil type.

## Results
*(Add your measured values here — e.g., moisture threshold used, response time from dry detection to watering, watering duration per cycle.)*

## Future Improvements
- Add Wi-Fi/IoT connectivity for remote monitoring and control
- Support multiple soil sensors for multi-plant setups
- Add a water level sensor for the reservoir to prevent dry-running the pump
- Integrate with a mobile app for watering schedule customization

## Author
Ayesha Ramzan — BS Electronics & Computing, COMSATS University Lahore
