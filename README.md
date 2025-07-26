💻 Alise McNiel | Tech Portfolio

👋🏾 I'm an IT tech and hands-on builder with a passion for embedded systems, smart automation, and cybersecurity. I use ESP32, Arduino, and C++ to bring my ideas to life — from touchscreen hacking tools to home automation dashboards.

🖥️ CM Box – ESP32 Touchscreen Terminal (Dell Linux Setup Guide)

This project sets up the CM Box hacking toolkit using the ESP32-2432S028R (C.Y.D.) board with a 2.8" resistive touchscreen. This guide walks through configuration on a Dell Ubuntu Linux system using Arduino IDE and CLI tools.

✅ What We Did

✅ Installed Arduino IDE 1.8.19 on Dell (Ubuntu)

✅ Installed ESP32 board definitions

✅ Installed required libraries like TFT_eSPI

✅ Switched TFT_eSPI config to use Setup249_ESP32_2432S028R

✅ Verified that User_Setup_Select.h correctly points to the CYD setup file

✅ Attempted multiple firmware uploads (Marauder & custom CM_Box firmware)

✅ Flashed .bin files using esptool.py and also prepped for web flasher

✅ Confirmed correct .bin file download and targeting the right COM port

✅ Verified compatibility with Dell’s Linux system for future debugging

⚙️ Dependencies

ESP32 Board Definitions: via Arduino Boards Manager

TFT_eSPI Library: manually configured

Python esptool.py for CLI flashing

Optionally: ESP Web Flasher for quick GUI flashing

🤖 NEPTUNE AI – Local Web Assistant (Ubuntu Setup Guide)

NEPTUNE is a custom local AI assistant that runs on your machine with voice input, voice output, and a glowing dark-mode web interface. It's designed for command mode workflows and automation.

✅ What We Did

✅ Created and activated a Python venv (neptune-venv)

✅ Built neptune.py Flask backend with provider switching (OpenAI / Groq)

✅ Loaded API keys securely via .env file

✅ Created animated frontend (HTML/JS/CSS) with mic button and dark glow UI

✅ Added voice-to-text with SpeechRecognition + PyAudio

✅ Added voice output using pyttsx3 and ElevenLabs API

✅ Built bridge_neptune_voice_eleven.py to connect mic → assistant → speech

✅ App runs locally at http://localhost:5000 with CORS enabled

⚙️ Dependencies

Flask (Backend)

SpeechRecognition, PyAudio (Mic input)

pyttsx3 or ElevenLabs API (Voice output)

Flask-CORS, dotenv, requests

Optional: Selenium + PyAutoGUI (job automation)

🧠 Notes

# Activate virtual environment
source neptune-venv/bin/activate

# Run the assistant
python3 neptune.py

Groq must return a choices field to avoid KeyError

ElevenLabs requires a valid API key

Ensure microphone permissions are enabled

🏠 SmartPad – ESP32 Smart Home System

A full-featured smart home automation prototype using sensors, relays, and a web dashboard.

✅ What We Did

✅ Connected DHT11 sensor to display live temp & humidity

✅ Set up PIR sensor to detect motion and trigger alerts

✅ Linked buzzer to motion for sound alarm

✅ Controlled external device with relay (e.g., fan/lamp)

✅ Built and served responsive web dashboard via ESP32

⚙️ Tech Stack

ESP32, DHT11, PIR Sensor, Relay Module, RGB LED

HTML/CSS/JS dashboard served via ESPAsyncWebServer

📸 Photos and video coming soon

🐾 TouchPet – Tamagotchi-Style Virtual Pet Game

Touchscreen-based pixel pet game with mood and hunger tracking.

✅ What We Did

✅ Designed sprite faces for happy, sad, tired, and hungry moods

✅ Programmed button interface to feed, play, or rest your pet

✅ Displayed real-time status via OLED

✅ Used OOP in C++ to structure pet behavior logic

⚙️ Tech Stack

ESP32, ILI9341 2.8" Touchscreen, TFT_eSPI, TouchLib

Object-oriented C++ game loop

📸 Gameplay and sprite animation preview coming soon

👁️ WatchCat – ESP32-CAM Motion Alert System

A mini surveillance system using ESP32-CAM and motion detection.

✅ What We Did

✅ Set up ESP32-CAM for live video stream

✅ Connected PIR sensor to detect motion

✅ Triggered visual LED alerts on motion

✅ Built test system for future cloud sync expansion

⚙️ Tech Stack

ESP32-CAM, PIR sensor, LED output

Arduino IDE with serial debugging

📸 Video feed snapshot and alert demo coming soon

🎛️ ControlBox v1 – Modular Sensor Panel

All-in-one dev rig with multiple inputs and outputs for sensor testing.

✅ What We Did

✅ Wired up joystick, buttons, and RFID module

✅ Added LCD1602 display for feedback

✅ Created flexible header system for swapping sensors

✅ Used for logic testing, I/O control, and classroom-style demos

⚙️ Tech Stack

ESP32, MFRC522 RFID, LCD1602, Joystick, Buttons

Wood panel mounted for portability

📸 Photos of sensor panel and test outputs coming soon

📚 DevBoard Library – Wiring + Codebase Templates

Collection of starter templates and wiring guides for rapid prototyping.

✅ What We Did

✅ Created reusable C++ functions for RGB, OLED, buzzer, etc.

✅ Made labeled diagrams for sensor pinouts

✅ Included example sketches for ultrasonic, temp/humidity, motion

✅ Added OTA example for updating firmware wirelessly

⚙️ Tech Stack

ESP32, Breadboard, OLED SSD1306, DHT11, HC-SR04, RGB LED, Arduino IDE

📸 Wiring diagrams and breadboard photos coming soon

💬 Freelance Availability

I build embedded systems and automation interfaces for personal, commercial, or educational projects.

💼 Services Offered:

Custom Arduino/ESP32 projects

Dashboard + UI development (touchscreen & web)

Debugging + code refactoring

Wiring diagrams + hardware prototyping

📧 Contact: mobileitsoulutions222@gmail.com

Let’s build something dope together 🚀

