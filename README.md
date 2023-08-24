# Accelerometer-Enhanced-GPS-Tracker
This repository contains a program for an IoT device that integrates various sensors to collect and transmit data. The device gathers temperature, touch, and accelerometer readings, along with GPS data, and sends them via a web request to a designated recipient. The program is written in Arduino language and is designed to run on compatible hardware.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Configuration](#setup-and-configuration)
- [Usage](#usage)
- [Sensors and Data](#sensors-and-data)
- [Author](#author)
- [License](#license)

## Features

- Collects temperature data in both Fahrenheit and Celsius from a temperature sensor.
- Retrieves touch sensor readings to indicate touch intensity.
- Captures accelerometer data to measure device motion in the X, Y, and Z axes.
- Integrates a GPS module to acquire altitude, satellite count, latitude, and longitude.
- Sends a web request to the CallMeBot API to deliver collected data.
- Smartly triggers data transmission when significant accelerometer readings are detected.
- Provides comprehensive information about device setup, sensors, and data transmission.

## Technologies Used

- Arduino Programming Language
- ESP8266 Microcontroller
- WiFi Connectivity
- Adafruit ADXL345 Accelerometer Library
- GPS Module Integration
- CallMeBot API for Message Transmission

## Setup and Configuration

1. Install the Arduino IDE (Integrated Development Environment).
2. Install required libraries for the ADXL345 accelerometer and the TinyGPS++ GPS module.
3. Connect the ESP8266 microcontroller and the sensors as indicated in the code.
4. Set your WiFi network credentials in the code: `ssid` and `password`.
5. Acquire an API key from the CallMeBot service and replace `"YOUR_API_KEY"` with the actual key.

## Usage

1. Upload the provided code to the ESP8266 microcontroller.
2. Observe the device collecting data and triggering transmission when accelerometer readings indicate motion.
3. Check the serial monitor for debug information and status updates.

## Sensors and Data

- **Temperature Sensor:** Reads the ambient temperature and provides values in both Fahrenheit and Celsius.
- **Touch Sensor:** Measures touch intensity and transmits the touch reading.
- **Accelerometer:** Captures acceleration data in the X, Y, and Z axes and sends the readings.
- **GPS Module:** Integrates altitude, satellite count, latitude, and longitude data.

## Author

Dhruv Singla

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code within the terms of the license agreement.
