# NOFUEL15(PATENT ACCEPTED)
An Automated Smart fueling System

App apk link - https://api.flutlab.io/projects/2564896/download-app?key=d6w4qnqif61ndzofbies&target=android-arm64

🚗 NOFUEL15 – Smart Fuel Authorization System
NOFUEL15 is an AI and IoT-based system designed to automate fuel control by blocking petrol or diesel supply to vehicles older than 15 years, in compliance with environmental regulations.

🧠 Problem Statement

Despite government bans on refueling vehicles over 15 years old, fuel stations lack any automated system to enforce this. Manual checks are inconsistent and inefficient, resulting in continued fuel supply to polluting, non-compliant vehicles.

✅ Solution Overview

NOFUEL15 uses a combination of hardware and software to:
- Capture vehicle number plate using ESP32-CAM
- Extract and verify number via OCR (EasyOCR + Python)
- Check vehicle age and VIN from a local or official database
- Control fuel flow via Arduino-controlled relay and solenoid valve
- Provide a mobile app (Flutter) for users to check eligibility
- Offer an admin dashboard for monitoring, override, and challan generation

 ⚙️ A patent has been filed for this innovation.

🧰 Tech Stack
Hardware:
- ESP32-CAM
- Arduino UNO
- Relay Module
- Solenoid Valve
- 16x2 I2C LCD

Software:
- Python (Flask + EasyOCR)
- Arduino IDE (C++)
- Flutter (User Mobile App)
- Firebase (optional, for app backend)
- HTML/CSS (Admin Dashboard UI)

Communication:
- Wi-Fi (App → Python Server)
- Serial (Python → Arduino)

🔄 User Flow

1. Vehicle arrives at petrol pump  
2. ESP32-CAM captures number plate  
3. Python extracts plate via OCR  
4. System checks vehicle age & VIN  
5. If valid → fuel allowed via Arduino  
6. If invalid → fuel blocked + challan  
7. Mobile app and dashboard show real-time status

🖥️ Admin Dashboard Features

- 🔴 Live camera feed  
- 📄 Scan history logs  
- ⚠️ Challan status and auto-generation  
- 🔐 Manual override for verified exceptions  
- 📊 Compliance reports  

📱 Mobile App Features (User)

- 🔍 Check vehicle fuel eligibility  
- 🧾 View challan details  
- 📆 Notifications on compliance status  

🔐 Security & Compliance

- Double verification: Number Plate + VIN  
- No personal data stored  
- Designed to align with VAHAN database format  
- Logs tampering attempts for auditing

📦 How to Run

1. Connect ESP32-CAM to local network
2. Run Python Flask server (`server.py`)
3. Upload Arduino code for relay control
4. Deploy Flutter app to Android device
5. Monitor system via dashboard

📜 License & IP

This project is protected under **patent filing status**. Unauthorized commercial use is prohibited without written permission.


