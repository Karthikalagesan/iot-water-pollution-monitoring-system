# 🌊 IoT-Based Water Pollution Monitoring System

An IoT-based water quality monitoring system developed as a Diploma in Electronic Engineering (Communication) project.

The system uses an ESP32 microcontroller, temperature and electrical conductivity (EC) sensors, an OLED display, and ThingSpeak to collect, display, and transmit water-quality-related measurements for remote monitoring

## 📌 Project Overview

The project was designed to provide a simple real-time approach to monitoring water quality parameters.

The implementation includes:

- 🌡️ Water temperature measurement
- ⚡ Electrical conductivity (EC) measurement
- 📟 OLED display for local readings
- 📡 ESP32 Wi-Fo connectivity
- ☁️ ThingSpeak cloud data transmission
- 🔄 Real-time data transmission
- 📊 Experimental data visualization

> **Note:** The original project documentation/flowchart also describes pH and turbidity monitoring. The source code currently included in this repository specifically implements temperature and EC measurement/transmission.

## 🛠️ Hardware

- ESP32 development board
- DS18B20 temperature sensor
- EC sensor
- ADS1115 ADC module
- 0.96-inch SSD1306 OLED display
- Water-quality sensing components
- Jumper wires and supporting circuitry

## 💻 Software & Libraries

- Arduino IDE
- C/C++ / Arduino
- ESP32 Wi-Fi
- ThingSpeak
- OneWire
- DallasTemperature
- DFRobot ESP EC
- Adafruit SSD1306
- Adafruit GFX
- Adafruit ADS1015

## ⚙️ System Operation

```text
Start
  ↓
Initialize ESP32, sensors, OLED and Wi-Fi
  ↓
Read temperature
  ↓
Read EC sensor voltage
  ↓
Calculate EC with temperature compensation
  ↓
Display temperature and EC on OLED
  ↓
Perform EC calibration
  ↓
Send readings to ThingSpeak
  ↓
Repeat
```

## 📊 Data Monitoring

The ESP32 sends the measured values to ThingSpeak:

- **Field 1:** Temperature
- **Field 2:** Electrical Conductivity (EC)

This allows the measurements to be monitored remotely through the ThingSpeak platform.

## 🔌 Source Code

The main Arduino source code is available in:

`iot-water-pollution-monitoring-system.ino`

## 📷 Project Documentation

Project images can be added to the `images/` folder, such as:

- Project front view
- Flowchart
- System output / ThingSpeak dashboard

## 🎓 Academic Project

**Programme:** Diploma in Electronic Engineering (Communication)  
**Institution:** Polytechnic Sultan Salahuddin Abdul Aziz Shah  
**Project Area:** IoT / Embedded Systems / Water Quality Monitoring

## 📚 Skills Demonstrated

- ESP32 programming
- Embedded systems
- Sensor interfacing
- Temperature measurement
- Electrical conductivity measurement
- OLED display interfacing
- Wi-Fi communication
- IoT cloud integration
- ThingSpeak data transmission
- Calibration
- Basic data monitoring and troubleshooting

## 🔐 Security Note

Wi-Fi credentials and ThingSpeak API credentials are intentionally replaced with placeholders in the source code. Do not publish real passwords or API keys on GitHub.

---

⭐ Developed as an academic engineering project focused on IoT-based environmental monitoring.
