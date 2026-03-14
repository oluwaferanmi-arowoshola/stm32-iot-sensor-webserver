# STM32 IoT Sensor Web Server

This project implements an embedded HTTP server on an STM32 IoT Discovery board that exposes temperature and humidity sensor data to a web browser over Wi-Fi.

## Features

- STM32 microcontroller firmware
- Temperature and humidity sensing
- Embedded HTTP server
- Wi-Fi networking
- Real-time sensor monitoring

## System Architecture

Temperature / Humidity Sensor
        ↓
     STM32 MCU
        ↓
   TCP/IP Stack
        ↓
    HTTP Server
        ↓
   Web Browser Client

## Hardware

STM32 B-L475E-IOT01A IoT Discovery Board

## Demonstration

The board prints its IP address through the serial terminal.  
A browser can connect to this address to display sensor data.
