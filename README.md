# STM32 IoT Sensor Web Server

This project implements an embedded HTTP server on an STM32 IoT Discovery board that exposes temperature and humidity sensor data to a web browser over Wi-Fi.

The firmware reads environmental data from onboard sensors and serves the values through a lightweight HTTP server. A client device such as a laptop or smartphone can connect to the board’s IP address and view the sensor readings directly in a web browser.

---

## Features

- Embedded firmware developed for STM32 microcontroller
- Real-time temperature and humidity sensing
- HTTP web server running on the microcontroller
- Wi-Fi connectivity for browser-based monitoring
- Serial debugging using ST-Link Virtual COM port

---

## System Architecture

![System Architecture](docs/system_architecture.png)

---

## Hardware

STM32 B-L475E-IOT01A IoT Discovery Board

Key hardware components used:

- STM32L475 microcontroller
- Onboard temperature sensor
- Onboard humidity sensor
- Wi-Fi module
- ST-Link debugger interface

---

## Firmware Overview

The firmware performs the following tasks:

1. Initialize STM32 peripherals and board support package  
2. Initialize the Wi-Fi networking stack  
3. Acquire temperature and humidity sensor data  
4. Launch an embedded HTTP server  
5. Serve real-time sensor values to connected web clients  

Primary firmware implementation:

firmware/main.c

Responsibilities include:

- Sensor data acquisition  
- Network initialization  
- HTTP response generation  
- Serial debugging output  

---

## Demonstration

When the firmware runs, the board prints its assigned IP address through the serial terminal.

Example serial output:

WiFi Connected  
IP Address: 192.168.35.11  
HTTP Server Started

A client can open a browser and navigate to the printed IP address to access the sensor web interface.

Example browser output:

Temperature: 24°C  
Humidity: 45%

---

## Development Environment

- STM32CubeIDE  
- C programming language  
- Tera Term serial terminal  

---

## Future Improvements

Possible extensions include:

- HTTPS support  
- REST APIs for sensor data  
- Mobile monitoring application  
- Cloud data logging  

---

## Author

Oluwaferanmi Arowoshola  
Electrical & Computer Engineering  
Minnesota State University, Mankato
