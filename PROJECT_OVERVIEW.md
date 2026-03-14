# Project Overview

This project demonstrates the design of a lightweight IoT monitoring system built using an STM32 microcontroller.

The system integrates environmental sensing, wireless networking, and embedded web services to provide real-time sensor monitoring through a standard web browser.

## Project Goals

The goal of the project was to explore several key embedded systems concepts:

* microcontroller firmware development
* sensor data acquisition
* Wi-Fi networking on embedded platforms
* embedded HTTP server implementation
* real-time system debugging

## System Operation

The STM32 firmware performs a continuous sensing and communication loop.

1. The microcontroller initializes onboard sensors and networking interfaces.
2. Environmental data is periodically sampled from the temperature and humidity sensors.
3. The embedded HTTP server listens for incoming client connections.
4. When a client sends an HTTP request, the firmware generates a response containing the most recent sensor readings.

The result is a simple browser-based interface that allows users to monitor environmental conditions directly from the embedded device.

## Engineering Concepts Demonstrated

This project demonstrates several important embedded systems concepts:

* peripheral initialization and configuration
* sensor interfacing on microcontrollers
* wireless communication using embedded networking stacks
* embedded web services on resource-constrained systems
* real-time debugging through serial interfaces

## Potential Applications

This architecture can be extended to many real-world IoT applications including:

* environmental monitoring systems
* smart building sensors
* industrial monitoring devices
* home automation sensors
