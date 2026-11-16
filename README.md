# EV-Wireless-Charging-IoT-
# Intelligent Wireless Power Transfer for EVs – An IoT-Based Approach

An IoT-enabled Electric Vehicle Wireless Charging System using Inductive Wireless Power Transfer (IWPT), IR-based misalignment detection, Arduino-based monitoring and ESP8266 cloud connectivity.

## 1. Project Overview

Electric vehicles require convenient, efficient and reliable charging solutions. Conventional plug-in charging requires manual connections and can cause cable wear and inconvenience.

This project proposes an intelligent wireless charging system that transfers power between transmitter and receiver coils using electromagnetic induction.

The system also incorporates IR-based misalignment detection and IoT-based monitoring to improve charging convenience, monitoring and safety.

## 2. Problem Statement

Conventional EV charging systems have certain limitations:

- Manual connection is required in plug-in charging.
- Coil misalignment can reduce wireless power transfer efficiency.
- Charging parameters are not always available for real-time monitoring.
- Users may not receive immediate alerts about charging conditions.

## 3. Proposed Solution

The proposed system integrates:

- **Wireless Power Transfer:** Transfers energy through inductive coupling between transmitter and receiver coils.
- **Misalignment Detection:** Uses an IR proximity sensor to detect the alignment condition and activate an alert.
- **Parameter Monitoring:** Arduino monitors voltage and current measurements.
- **IoT Connectivity:** ESP8266 sends monitoring data to the ThingSpeak cloud platform.
- **User Interface:** OLED display and web dashboard provide charging information.

## 4. System Architecture

```text
    Transmitter Coil
           |
    Magnetic Coupling
           |
     Receiver Coil
           |
     EV Charging Unit

 IR Sensor --------|
 Current Sensor ---|
 Voltage Sensor ---|
                   |
              Arduino UNO
                   |
       +-----------+-----------+
       |           |           |
     Buzzer      OLED       ESP8266
                              |
                           Wi-Fi
                              |
                         ThingSpeak
                              |
                        Web Dashboard
```

## 5. Hardware Components

| Component | Purpose |
|---|---|
| Arduino UNO | Main controller |
| IR Proximity Sensor | Misalignment detection |
| ACS712 Current Sensor | Current measurement |
| Voltage Sensor | Voltage measurement |
| Buzzer | Alert indication |
| OLED Display | Local parameter display |
| ESP8266 Wi-Fi Module | IoT connectivity |
| Transmitter Coil | Wireless power transmission |
| Receiver Coil | Wireless power reception |

## 6. Software and Technologies

- Programming Language: Embedded C/C++ (Arduino)
- Development Environment: Arduino IDE
- Microcontroller Platform: Arduino UNO
- IoT Platform: ThingSpeak
- Communication: Wi-Fi using ESP8266

## 7. Working Methodology

1. The transmitter coil generates an alternating magnetic field.
2. The receiver coil receives energy through electromagnetic induction.
3. The IR proximity sensor monitors the alignment condition.
4. When misalignment is detected, the buzzer alerts the user.
5. Arduino collects voltage and current sensor readings.
6. The monitoring data is sent through ESP8266.
7. ThingSpeak provides cloud-based data monitoring.
8. Charging information is displayed locally and remotely.

## 8. Key Features

- Inductive wireless power transfer.
- IR-based misalignment detection.
- Audible alert for alignment issues.
- Voltage and current monitoring.
- OLED-based local display.
- IoT-based remote monitoring.
- ThingSpeak cloud integration.

## 9. Applications

- Electric vehicle charging stations.
- Smart roads and highways.
- Electric vehicle fleet management.
- Automated guided vehicles.
- Wireless charging research and development.

## 10. Future Improvements

- Automatic coil alignment using motorized positioning.
- Advanced charging efficiency optimization.
- Battery state-of-charge monitoring.
- Enhanced safety and fault detection.
- Mobile application integration.

## 11. Repository Structure

```text
EV-Wireless-Charging-IoT/
│
├── README.md
├── Source-Code/
│   ├── Arduino/
│   └── ESP8266/
├── Documentation/
├── Presentation/
├── Images/
└── LICENSE
```

## 12. Contributors

- Charulatha G
- Yuvashree

*Please retain contributor names according to the actual project contributions.*

## 13. Project Information

**Project Title:** Intelligent Wireless Power Transfer for EVs: An IoT-Based Approach

**Domain:** Electrical and Electronics Engineering, IoT and Embedded Systems

**Technologies:** Arduino, Embedded C/C++, ESP8266, ThingSpeak and Inductive Wireless Power Transfer.

---

*This repository documents the project design, implementation resources and technical development of an IoT-based wireless EV charging prototype.*
