# Smarter Agriculture: IoT Palm Tree Monitoring & Management System

## 📋 Project Overview
This project presents a comprehensive IoT and sensor-based solution designed to optimize agricultural management and evaluate the ecological impact of palm tree farms (specifically developed for Nakhla Company). The system utilizes a wireless sensor network to autonomously track vital agricultural metrics, automate farming processes, and upload real-time data to cloud platforms.

## ✨ Key Features
*   **Ecological CO2 Tracking:** Measures the amount of Carbon Dioxide (CO2) absorbed by palm trees using MQ-135 gas sensors to evaluate their role in reducing environmental pollution.
*   **Soil Nutrient Analysis:** Monitors Nitrogen, Phosphorus, and Potassium (NPK) levels in the soil using an RS485 NPK sensor to accurately estimate fertilizer requirements.
*   **Automated Smart Irrigation:** Utilizes soil moisture sensors and relays to autonomously control water pumps, ensuring irrigation only occurs when the soil is dry, thereby preventing water waste.
*   **Phenology Prediction:** Tracks ambient temperature using DHT11 and LM35 sensors to calculate accumulated thermal units, which helps in predicting precise flowering and fruit ripening dates.
*   **IoT Cloud Integration:** Transmits gathered telemetry data wirelessly to centralized platforms, including Excel spreadsheets and the ThingSpeak IoT platform, enabling real-time monitoring and data visualization.

## 📡 System Architecture
As illustrated in the system diagram, the network operates using a dual-node wireless configuration:
*   **Transmitter Node:** Powered by a solar panel, this node uses an Arduino Uno equipped with MQ-135 and DHT11 sensors to collect localized environmental data, which is then broadcasted via an XBee (Zigbee) RF module.
*   **Receiver & Gateway Node:** Also solar-powered, this secondary Arduino node receives the XBee transmission from up to 120 meters away. It collects its own local sensor data and utilizes an ESP32 (NodeMCU) Wi-Fi module to push the aggregated data to the internet router for cloud storage.

## 🛠 Hardware Components
*   **Microcontrollers & Communications:** Arduino Uno, Digi XBee S2C (Zigbee), ESP32 (NodeMCU) Wi-Fi Module, and SIM800L GSM Module (for SMS alerts).
*   **Sensors:** MQ-135 Gas Sensor, DHT11 Temperature & Humidity Sensor, RS485 Soil NPK Sensor, Soil Moisture Sensor, and LM35 Temperature Sensor.
*   **Power & Actuation:** Solar Panels (e.g., 25V / 12V 60W), DC Water Pump Motor, DC Cooling Fan, and Relays.

## 👨‍💻 Project Team
This system was designed and developed by the "Smarter Agriculture" team from the Northern Technical University (NTU).
