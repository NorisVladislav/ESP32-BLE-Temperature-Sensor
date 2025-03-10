# ESP32-BLE-Temperature-Sensor

# Project: Temperature Sensor with Bluetooth Interface using Arduino and Phyphox

## Description
This project involves building a wireless temperature monitoring system using an Arduino-compatible board and a DS18B20 sensor. The system transmits real-time temperature data to a mobile device via Bluetooth Low Energy (BLE) and displays it in the Phyphox mobile application.

The main goal is to create a simple yet efficient solution for remote temperature monitoring, which can be used for various applications, such as home automation, environmental monitoring, and educational purposes.

## Features
- ✅ Wireless temperature monitoring via Bluetooth Low Energy (BLE)
- ✅ Real-time temperature readings displayed in the Phyphox app
- ✅ Compatible with multiple devices (ESP32, Arduino with BLE modules, etc.)
- ✅ Low power consumption for continuous operation
- ✅ Customizable and extendable for additional functionalities

## Components & Requirements

### Hardware:
- Arduino development board (e.g., ESP32)
- DS18B20 temperature sensor
- 4.7kΩ pull-up resistor (required for DS18B20)
- Breadboard and jumper wires
- Mobile device with Bluetooth Low Energy (BLE) support

### Software:
- Arduino IDE
- Phyphox mobile application (available on iOS & Android)
- DallasTemperature & OneWire libraries for DS18B20

## Installation & Usage

### 1. Hardware Setup
- Connect the VCC pin of the DS18B20 sensor to 3.3V (or 5V) on the Arduino.
- Connect the GND pin to GND.
- Connect the DATA pin to a digital input (e.g., GPIO4 on ESP32).
- Place a 4.7kΩ pull-up resistor between VCC and DATA.

### 2. Software Setup
- Install the Arduino IDE and add the necessary libraries:
  - OneWire (for communication with the sensor)
  - DallasTemperature (for handling DS18B20)
- Upload the provided Arduino code to your board.
- Open the Phyphox app on your mobile device.

### 3. Connecting to Bluetooth
- Ensure Bluetooth is enabled on your phone.
- In Phyphox, search for available Bluetooth devices.
- Select the device named "ESP32" (or the custom name set in your code).
- Once connected, the app will start receiving and displaying real-time temperature data.

## Customization & Expansion
- Modify the Arduino code to log data to an SD card or send alerts when temperature exceeds a threshold.
- Add multiple sensors to monitor different locations.
- Integrate with cloud platforms (such as Firebase, ThingSpeak) for remote data access.
- Use a battery-powered setup for portability.

## Troubleshooting
⚠️ **Device not connecting?** Ensure Bluetooth is enabled and BLE is supported.  
⚠️ **No temperature readings?** Check wiring, pull-up resistor, and sensor connections.  
⚠️ **Incorrect readings?** Ensure the DS18B20 sensor is functioning correctly and properly powered.

## Possible Applications
- 📡 **Home automation** – Monitor room temperature remotely.
- 🌱 **Greenhouse monitoring** – Maintain optimal temperature for plant growth.
- 🚗 **Automotive applications** – Measure engine or cabin temperature.
- 🏠 **Smart HVAC systems** – Improve heating and cooling efficiency.

## License
This project is open-source and can be freely modified and shared.

## Author
Vladislav Noris - Victor
