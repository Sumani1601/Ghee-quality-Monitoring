# 🧈 IoT-Based Ghee Quality Monitoring System

## 📌 Project Overview

The **IoT-Based Ghee Quality Monitoring System** is a smart system designed to monitor and classify the quality of ghee based on environmental and chemical parameters.

The system uses an **ESP32 microcontroller** along with sensors to collect parameters such as **temperature, humidity, moisture, and gas levels**. Based on the sensor readings, the ghee is classified into different quality grades.

## 🎯 Objective

The main objective of this project is to develop a low-cost and efficient system that can provide **quick and automated ghee quality assessment** without relying completely on traditional manual inspection methods.

## ⚙️ Technologies Used

* **ESP32** – Main microcontroller
* **DHT11 Sensor** – Temperature and humidity measurement
* **Moisture Sensor** – Moisture-level detection
* **Gas Sensor** – Detection of gas/volatile compounds
* **16×2 I2C LCD** – Displays sensor readings and quality grade
* **Bluetooth Serial Communication** – Transfers sensor data
* **Arduino IDE** – Programming and development
* **Embedded C/C++** – Microcontroller programming

## 🔄 Working Principle

1. The ghee sample is placed near the sensing unit.
2. Sensors collect relevant parameters such as temperature, humidity, moisture, and gas level.
3. The **ESP32** processes the sensor readings.
4. The measured values are compared with predefined quality conditions.
5. Based on the readings, the system classifies the ghee as:

   * 🟢 **Grade A – Good Quality**
   * 🟡 **Grade B – Average Quality**
   * 🔴 **Grade C – Poor Quality**
6. The quality grade and sensor values are displayed on the LCD.
7. Sensor data can also be transmitted through Bluetooth for monitoring.

## 🧩 System Architecture

```text
             Ghee Sample
                  │
                  ▼
        ┌───────────────────┐
        │      Sensors      │
        │                   │
        │ DHT11             │
        │ Moisture Sensor   │
        │ Gas Sensor        │
        └─────────┬─────────┘
                  │
                  ▼
        ┌───────────────────┐
        │       ESP32       │
        │ Data Processing & │
        │ Quality Analysis  │
        └───────┬─────┬─────┘
                │     │
          ┌─────▼─┐ ┌─▼──────────┐
          │ LCD   │ │ Bluetooth  │
          │Display│ │ Monitoring │
          └───────┘ └────────────┘
                  │
                  ▼
          Quality Classification
          Grade A / Grade B / Grade C
```

## ✨ Key Features

* Automated ghee quality monitoring
* Multiple sensor-based measurements
* Real-time display of sensor readings
* Automatic quality classification
* Bluetooth-based data communication
* Low-cost IoT-based implementation
* Easy-to-use monitoring system

## 🛠️ Hardware Components

| Component       | Purpose                          |
| --------------- | -------------------------------- |
| ESP32           | Data processing and control      |
| DHT11           | Temperature and humidity sensing |
| Moisture Sensor | Moisture measurement             |
| Gas Sensor      | Gas/volatile compound detection  |
| 16×2 I2C LCD    | Displaying readings and results  |
| Power Supply    | Provides power to the system     |

## 📊 Output

The system provides sensor readings and determines the corresponding quality grade of the ghee.

Example:

```text
Temperature : XX °C
Humidity    : XX %
Moisture    : XX
Gas Level   : XX

Ghee Quality: Grade A
```

## 🚀 Future Improvements

* Develop a larger dataset of ghee samples.
* Apply **Machine Learning** for more accurate quality classification.
* Add cloud-based data storage and monitoring.
* Develop a mobile/web dashboard for real-time monitoring.
* Improve sensor calibration and testing with laboratory-verified samples.
* Extend the system to detect adulteration and spoilage indicators.

## 👩‍💻 Project

**Project:** IoT-Based Ghee Quality Monitoring System
**Domain:** Internet of Things (IoT) / Embedded Systems
**Controller:** ESP32
**Programming:** C/C++
**Development Platform:** Arduino IDE

---

### 📄 Portfolio

A detailed project portfolio is available in:

`ghee_quality_monitoring_portfolio.html`

You can open the HTML file from this repository to view the project presentation and details.
