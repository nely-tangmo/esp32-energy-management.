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
---

# Version française

# Système embarqué ESP32 de mesure électrique et de télésurveillance des charges (MQTT)

Projet d'équipe de Master 1 EEA (8 étudiants), Département de Physique, Université de Dschang, Cameroun (2025/2026). Encadrant : Pr Hilaire Fotsin.

## Présentation
Système embarqué basé sur l'ESP32 qui mesure les paramètres électriques d'une installation et permet de surveiller et de commander à distance trois charges électriques via le protocole MQTT. Il vise les petits locaux et habitations où la supervision énergétique est absente ou trop coûteuse.

## Fonctionnalités
- Mesure de la tension, du courant, de la puissance active, de l'énergie consommée, de la fréquence du réseau et du facteur de puissance (capteur PZEM-004T V3, avec isolation galvanique)
- Commande à distance de 3 charges par relais, et commande locale par 3 boutons poussoirs
- Protection automatique (surtension, sous-tension, fréquence anormale) avec reconnexion au retour à la normale
- Affichage local sur un écran TFT ILI9341 3,5" : mesures, état des charges, énergie journalière et mensuelle, priorité des charges, alertes
- Envoi des données en temps réel via MQTT sécurisé (TLS) vers un broker cloud (HiveMQ Cloud)
- Interface web de supervision (HTML5 / JavaScript, WebSocket sécurisé) avec courbes en temps réel, journal d'événements, commande à distance et alertes

## Technologies
- Matériel : ESP32, PZEM-004T V3, relais, contacteur, écran TFT, boutons poussoirs
- Logiciel embarqué : C/C++ (Arduino IDE), bibliothèques PubSubClient, PZEM004Tv30, Arduino_GFX, ArduinoJson, EEPROM, heure NTP
- Protocoles : Wi-Fi, MQTT sur TLS, WebSocket sécurisé

## Coût
Environ 94 500 FCFA pour le prototype principal, une alternative économique aux systèmes de supervision industriels.

## Ma contribution
Projet d'équipe. Ma part : rédaction du rapport final, contribution à la présentation du projet et une partie du câblage.

## Perspectives
Application mobile, module GSM/4G, stockage des données dans le cloud, alimentation solaire, analyse par intelligence artificielle.
