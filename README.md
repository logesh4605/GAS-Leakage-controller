🚨 GSM-Based LPG Gas Leak Detection & Auto Shut-off System

A smart embedded safety system designed to detect LPG gas leakage, automatically shut off the gas supply, trigger local alarms, and notify users remotely using GSM communication. This project demonstrates the integration of sensors, actuators, and wireless communication for real-time industrial and residential safety applications.

---

📌 Overview

LPG gas leakage is one of the major causes of domestic and industrial fire accidents. This project continuously monitors gas concentration using an MQ-2 gas sensor. When the detected gas level exceeds a predefined threshold, the system immediately:

- Detects LPG gas leakage
- Activates a buzzer and warning LED
- Automatically closes the gas regulator using a servo motor
- Sends an SMS alert to the registered mobile number
- Places an emergency phone call through a GSM module

The system is built using Arduino and is suitable for smart home and industrial safety applications.

---

✨ Features

- 🔥 Real-time LPG gas leak detection
- 📱 SMS alert using GSM module
- 📞 Automatic emergency phone call
- ⚙️ Automatic gas valve shut-off using Servo Motor
- 🚨 Buzzer and LED warning indicators
- 🛡️ Prevents repeated SMS alerts for the same leakage event
- 🔄 Automatically resets after gas concentration returns to a safe level

---

🛠️ Hardware Components

Component| Quantity
Arduino Uno| 1
MQ-2 Gas Sensor| 1
GSM Module (SIM800L/SIM900A)| 1
Servo Motor (SG90/MG90S)| 1
Relay Module| 1
Buzzer| 1
LED| 1
Jumper Wires| As Required
Breadboard / PCB| 1
External Power Supply| 1

---

💻 Software Used

- Arduino IDE
- Embedded C / Arduino Programming
- SoftwareSerial Library
- Servo Library

---

⚙️ Working Principle

1. The MQ-2 sensor continuously monitors LPG gas concentration.
2. Arduino reads the analog sensor value.
3. If the gas level exceeds the threshold:
   - Relay is activated.
   - Buzzer starts sounding.
   - LED turns ON.
   - Servo rotates to close the gas regulator.
   - GSM module sends an SMS alert.
   - GSM module makes an emergency phone call.
4. Once the gas level becomes safe:
   - Alarm stops.
   - LED turns OFF.
   - Relay deactivates.
   - Servo reopens the regulator.
   - System resumes monitoring.

---

📂 Project Structure

📁 GSM-Gas-Leak-Detection
│
├── GSM_Gas_Leak_Detection_System.ino
├── README.md
├── circuit_diagram.png
├── hardware_setup.jpg
└── images/

---

🔧 Pin Configuration

Device| Arduino Pin
MQ-2 Sensor| A0
Servo Motor| D9
Relay Module| D10
Buzzer| D6
LED| D13
GSM RX| D7
GSM TX| D8

---

📲 GSM Functions

The GSM module performs:

- AT Command Initialization
- SMS Transmission
- Emergency Voice Call

Example Alert:

WARNING!
LPG GAS LEAK DETECTED.

---

🚀 Future Improvements

- IoT monitoring using ESP32
- Mobile application integration
- Cloud dashboard (ThingSpeak/Blynk)
- Gas concentration graph
- Battery backup system
- Multiple gas sensor support
- Fire and smoke detection integration

---

🎯 Applications

- Smart Homes
- LPG Storage Facilities
- Restaurants
- Hotels
- Laboratories
- Industrial Plants
- Chemical Industries

---

📚 Technologies Used

- Embedded Systems
- Arduino Programming
- GSM Communication
- Sensor Interfacing
- Automation
- Safety Monitoring

---

👨‍💻 Author

Logeshwaran G

Electronics and Communication Engineering (ECE)

Aspiring Embedded Systems Engineer

---

⭐ If you found this project useful

Please consider giving this repository a ⭐ Star to support the project.
