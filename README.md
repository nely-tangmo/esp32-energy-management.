# ESP32 Smart Electrical Monitoring and Remote Load Control (MQTT)  Master 1 EEA team project (8 students), Department of Physics, University of Dschang, Cameroon (2025/2026). Supervisor: Prof. Hilaire Fotsin. 
## Overview
An embedded system based on the ESP32 that measures the electrical parameters of an installation and allows remote monitoring and control of three electrical loads over the MQTT protocol. It targets small homes and premises where energy supervision is missing or too expensive.
## Features
- Measurement of voltage, current, active power, energy consumed, grid frequency and power factor (PZEM-004T V3 sensor, galvanic isolation) - Remote control of 3 loads through relays, plus local control with 3 push buttons - Automatic protection (overvoltage, undervoltage, abnormal frequency) with reconnection once values return to normal - Local display on a 3.5" ILI9341 TFT screen: measurements, load states, daily and monthly energy, load priority, alerts - Real-time data sent over MQTT with TLS to a cloud broker (HiveMQ Cloud) - Web dashboard (HTML5 / JavaScript, secure WebSocket) with live curves, event log, remote control and alerts
## Tech stack
Hardware: ESP32, PZEM-004T V3, relays, contactor, TFT display, push buttons - Firmware: C/C++ (Arduino IDE), libraries PubSubClient, PZEM004Tv30, Arduino_GFX, ArduinoJson, EEPROM, NTP time - Protocols: Wi-Fi, MQTT over TLS, WebSocket Secure  
## Cost 
About 94,500 FCFA for the main prototype, a low-cost alternative to industrial supervision systems.  
## My contribution Team project.
My part: writing the final project report, contributing to the project presentation, and part of the hardware wiring.  
## Future improvements Mobile app, GSM/4G module, cloud data storage, solar power supply, AI-based analysis.
