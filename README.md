# Laser Security System Using IoT
## Overview
The Laser Security System Using IoT is an Arduino-based project that combines laser detection technology with Internet of Things (IoT) to create an intelligent and remotely accessible security system. The system integrates an ESP32-CAM module, a laser, and a Telegram bot for efficient monitoring and control.

## Project Features
Laser Detection Technology: Utilizes laser beams for accurate intrusion detection.

### IoT Integration: 
Connects to Telegram bot for real-time monitoring and control.

### Remote Commands:
Interact with the ESP32-CAM through Telegram commands.

### Photo Capture:
Capture photos on demand and send them to a Telegram chat.

### Flash LED Control:
Toggle the flash LED for additional illumination.

## Hardware Requirements
* ESP32-CAM module
* Laser module
* LDR (Light Dependent Resistor)
* Arduino board
* WiFi module
* Telegram Bot API Token
* Wiring Instructions
* Connect the laser module to pin 12 (LaserPin).
* Connect the LDR to pin 13 (LDRPin).
* Connect the flash LED to pin 4 (FlashLEDPin).
* Ensure proper connections for the ESP32-CAM module.

## Arduino Libraries

### Ensure the following Arduino libraries are installed:
* WiFi.h
* WiFiClientSecure.h
* UniversalTelegramBot.h
* ArduinoJson.h
  
## Configuration
Set your WiFi credentials: const char* ssid = "YourWiFiSSID"; and const char* password = "YourWiFiPassword";
Set your Telegram bot token: String BOTtoken = "YourBotToken";
Set your Telegram chat ID: String CHAT_ID = "YourChatID";
## Usage
Flash the code to the ESP32-CAM module.
Open the Serial Monitor to view system messages.
Interact with the ESP32-CAM via Telegram commands.
## Telegram Commands
/start: Displays welcome message and available commands.
/photo: Takes a new photo and sends it to the Telegram chat.
/flash: Toggles the flash LED on/off.
/laseron: Turns on the laser.
/laseroff: Turns off the laser.
## Acknowledgments
Credits to the authors of libraries used in this project.
