# 💻 Alise McNiel | Tech Portfolio

👋🏾 I'm an IT tech and hands-on builder with a passion for embedded systems, smart automation, and cybersecurity. I use ESP32, Arduino, and C++ to bring my ideas to life — from touchscreen hacking tools to home automation dashboards.

---

# CM Box (ESP32 Touchscreen Terminal) – Dell Setup Guide 🖥️⚡

This project sets up the CM Box hacking toolkit using the **ESP32-2432S028R (C.Y.D.) board** with a **2.8" resistive touchscreen**. This README covers setup on a **Dell Linux laptop**, using Arduino IDE with custom TFT settings.

---

## ✅ What We Did

- ✅ Installed Arduino IDE 1.8.19 on Dell (Ubuntu)
- ✅ Installed ESP32 board definitions
- ✅ Installed required libraries like `TFT_eSPI`
- ✅ Switched `TFT_eSPI` config to use **Setup249_ESP32_2432S028R**
- ✅ Verified that `User_Setup_Select.h` correctly points to the CYD setup file
- ✅ Attempted multiple firmware uploads (Marauder & custom CM_Box firmware)
- ✅ Flashed `.bin` files using `esptool.py` and also prepped for web flasher
- ✅ Confirmed correct `.bin` file download and targeting the right COM port
- ✅ Verified compatibility with Dell’s Linux system for future debugging

---

## 🛠 Dependencies

- **ESP32 Board Definitions**: via Arduino Boards Manager  
- **TFT_eSPI Library**: manually configured
- **Python `esptool.py`** for CLI flashing
- Optionally: [ESP Web Flasher](https://esphome.github.io/esp-web-tools/) for quick GUI flashing

---

 🤖 NEPTUNE AI (Local Web Assistant) – Ubuntu Setup Guide 🤖🔫

This project builds a local AI assistant named NEPTUNE, running on a custom web interface with voice input/output. It uses a Flask backend, a glowing dark-themed HTML/JS frontend, and supports both OpenAI and Groq API providers.

Built and tested on a Dell Ubuntu Linux laptop.

✅ What We Did

🔳 Installed Flask and Python dependencies in virtual environment (neptune-venv)

🔳 Built custom Flask server (neptune.py) with:

Provider switching (OpenAI / Groq)

.env file loading for API keys

🔳 Created a glowing dark mode UI:

Input field, mic button, and send button

Dropdown menu to select provider

🔳 Added voice-to-text with SpeechRecognition + PyAudio

🔳 Added voice output using pyttsx3 and ElevenLabs TTS

🔳 Enabled /ask endpoint to return and speak AI replies

🔳 Created bridge_neptune_voice_eleven.py to link mic input to assistant

🔳 App runs smoothly at http://localhost:5000 with CORS enabled

🛠 Dependencies

Flask for backend server

SpeechRecognition, PyAudio for mic input

pyttsx3 or elevenlabs for voice output

Flask-CORS to enable local dev mode

python-dotenv to load API keys securely

Optional: Selenium + PyAutoGUI for job automation

🧠 Notes

# Activate virtual environment
source neptune-venv/bin/activate

# Run the assistant
python3 neptune.py

The Groq provider must return a "choices" field or will cause a KeyError

ElevenLabs speech won’t work without a valid API key

Confirm microphone permissions if speech fails

Designed for local offline/online hybrid assistant workflows. Can be expanded to job automation, sensor interfacing, and AI agent control.


🔧 Embedded Systems Portfolio – ESP32 Projects

Welcome to my collection of embedded systems projects built with ESP32, Arduino, and touchscreen interfaces. These are hands-on demos blending IoT, sensors, automation, and creative interfaces—perfect for showing off both software and hardware skills.
🏠 SmartPad – ESP32 Smart Home System

A fully functional smart home demo that showcases real-time automation and environmental tracking.
💡 Features:

    PIR motion detection triggers alerts and RGB LED effects

    DHT11 sensor reports temperature & humidity live to the web UI

    Buzzer alarms when unauthorized movement is detected

    Relay module controls external devices (e.g., lights or fans)

    Responsive web dashboard served from ESP32 (HTML/CSS/JS)

🧰 Tech Stack:

ESP32, DHT11, PIR sensor, Relay, RGB LED, Web Server (ESPAsync), Arduino IDE

📸 Demo video and screenshots coming soon
🐾 TouchPet – Virtual Pet Game (Tamagotchi Clone)

A pixel-style pet game with touchscreen interaction and mood simulation.
🐱 Features:

    Interactive touchscreen buttons for feeding, playing, and checking mood

    Animated sprites change based on pet’s happiness, hunger, and rest

    OLED screen displays pet's expressions and real-time status

    Built as a mini-game engine in C++ using object-oriented design

🧰 Tech Stack:

ESP32, ILI9341 2.8" Touchscreen, TFT_eSPI, TouchLib, C++

📸 Gameplay video and sprite animations coming soon
👁️ WatchCat – ESP32-CAM Motion Surveillance

An IoT-based security prototype using a camera and motion sensor.
🛡️ Features:

    ESP32-CAM live streaming feed

    PIR motion sensor triggers a flashing LED alert

    Expansion-ready for cloud notifications or image capture

    Great for experimenting with ESP32-CAM automation logic

🧰 Tech Stack:

ESP32-CAM, PIR Sensor, GPIO-controlled LEDs, Arduino IDE

📸 Video capture and alert test shots on the way
🎛️ ControlBox v1 – Modular Sensor Testing Rig

A versatile dev board setup with multiple sensor modules and controls.
⚙️ Features:

    Joystick, buttons, RFID scanner, and LCD output

    Easy-swappable design with pin headers for testing new components

    Used to prototype input/output handling, serial comms, and modular logic

    Mounted on a wooden panel for portability and workspace organization

🧰 Tech Stack:

ESP32, MFRC522 RFID, LCD1602, Joystick, Pushbuttons, C++

📸 Workspace pics and demo interactions coming soon
📚 DevBoard Library – ESP32 Code & Wiring Templates

A ready-to-use library of sample code and hookup diagrams.
🧩 Features:

    Reusable C++ functions for buzzer tones, RGB LED animation, and OLED text

    Pinout-ready examples for HC-SR04, PIR, Temp/Humidity, Light sensors

    Basic web server templates and OTA update functions

    Modular structure for plugging into any new ESP32 or Arduino project

🧰 Tech Stack:

ESP32, Arduino IDE, Breadboard, DHT11, OLED SSD1306, Buzzer, RGB LED

📸 Preview images of breadboard setups and working demos coming soon

    💬 All codebases and diagrams are 100% beginner-friendly, with inline comments and serial debug output to help anyone build their own smart systems or test rigs from scratch.
