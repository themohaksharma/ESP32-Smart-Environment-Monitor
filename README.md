# ESP32 Smart Environment Monitor

An IoT-based temperature monitoring and remote device control system built using ESP32, an LM35 temperature sensor, and the Blynk IoT platform.

## Overview

The ESP32 Smart Environment Monitor is designed to monitor temperature in real time and provide remote control of connected electronic devices through a Blynk dashboard.

The ESP32 connects to a Wi-Fi network and communicates with Blynk Cloud, allowing users to monitor temperature readings and operate connected outputs remotely.

## Features

- Real-time temperature monitoring using an LM35 sensor.
- Wi-Fi connectivity through ESP32.
- Live temperature updates on a Blynk dashboard.
- Remote LED/light control.
- Remote buzzer control.
- Mobile and web-based monitoring through Blynk.

## Hardware Components

| Component | Purpose |
|---|---|
| ESP32 Development Board | Main microcontroller |
| LM35 Temperature Sensor | Temperature measurement |
| LED | Light output control |
| Buzzer | Audio output |
| Resistor | LED current limiting |
| Breadboard | Circuit assembly |
| Jumper Wires | Hardware connections |

## Pin Configuration

| Component | ESP32 GPIO |
|---|---|
| LM35 Output | GPIO 36 |
| LED | GPIO 13 |
| Buzzer | GPIO 17 |
| Status LED | GPIO 2 |

## Software & Technologies

- Arduino IDE
- Embedded C/C++ (Arduino framework)
- ESP32 Wi-Fi Library
- Blynk IoT Platform
- ESP_LM35 Library

## Blynk Dashboard

The project uses Blynk Virtual Pins for communication between the ESP32 and the dashboard.

| Virtual Pin | Function |
|---|---|
| V0 | Temperature readings |
| V1 | LED/Light control |
| V2 | Buzzer control |

The dashboard can display temperature readings and provide switches to control the connected LED and buzzer.

## Working Principle

1. The LM35 sensor measures the surrounding temperature.
2. The ESP32 reads the sensor output through GPIO 36.
3. The temperature value is sent to Blynk Cloud through Wi-Fi.
4. The dashboard displays the temperature in Celsius.
5. Users can control the LED and buzzer using dashboard switches.
6. The ESP32 receives the control commands and operates the corresponding GPIO pins.

## Setup Instructions

1. Install Arduino IDE.
2. Install the ESP32 board package.
3. Install the required Blynk and ESP_LM35 libraries.
4. Create a device template in Blynk Cloud.
5. Configure the required virtual datastreams.
6. Add your Wi-Fi credentials and Blynk device credentials to the sketch.
7. Select the appropriate ESP32 board and port.
8. Upload the sketch to the ESP32.

## Security Note

Wi-Fi credentials and Blynk authentication tokens should never be committed to a public repository.

Replace the placeholder credentials in the source code with your own private configuration before running the project.

## Future Improvements

- Add humidity monitoring.
- Introduce temperature threshold alerts.
- Add historical temperature graphs.
- Expand the system with additional environmental sensors.
- Improve dashboard visualization and device monitoring.

## Project Status

Initial implementation documented and source code published.

---

**Developed by:** [Mohak Sharma](https://github.com/themohaksharma)

**GitHub:** https://github.com/themohaksharma
