# 💻 Alise McNiel | Tech Portfolio

👋🏾 I'm an IT tech and hands-on builder with a passion for embedded systems, smart automation, and cybersecurity. I use ESP32, Arduino, and C++ to bring my ideas to life — from touchscreen hacking tools to home automation dashboards. Below are my featured projects built from the ground up, with a strong focus on real-world usability, creativity, and clean engineering.

---

# 🖥️ CM Box – ESP32 Touchscreen Terminal Toolkit (Dell Linux Setup)

A powerful and portable ESP32-based touchscreen terminal designed for hacking, diagnostics, and modular expansion. CM Box features a fully interactive UI, OTA support, and firmware flexibility with support for Marauder tools and custom modules.

---

## ✅ Key Features

* ✅ **Touchscreen UI** built using TFT\_eSPI with custom theme and icons
* ✅ **ESP32-2432S028R (C.Y.D.)** board with 2.8" resistive touch display
* ✅ Dual-mode firmware support (custom + Marauder)
* ✅ OTA-ready setup with `.bin` flashing via CLI and GUI
* ✅ Built on **Dell Ubuntu Linux** for real-time debugging and serial monitoring
* ✅ Designed to be expanded with GPS, Evil Portal, BLE sniffing, and more

---

## 🛠️ Setup Process

* Installed Arduino IDE 1.8.19
* Installed and configured ESP32 board definitions via Board Manager
* Customized `TFT_eSPI` config to match Setup249\_ESP32\_2432S028R
* Verified `User_Setup_Select.h` points to the CYD board setup file
* Flashed `.bin` firmware using Python `esptool.py`
* Tested multiple firmware packages (Marauder, CM\_Box\_UI)
* Setup Web Flasher compatibility for user-friendly flashing

---

## ⚙️ Tech Stack

* ESP32 (C.Y.D. 2432S028R)
* TFT\_eSPI, Arduino IDE, esptool.py, Bash
* PlatformIO (optional), OTA ready

📸 *UI screenshots, terminal testing, and demo videos coming soon*

---

# 🤖 NEPTUNE AI – Local Voice-Driven Web Assistant

NEPTUNE is a hybrid offline/online personal assistant with a dark-mode browser interface, voice recognition, and AI-powered responses. Designed to automate workflows, interact with sensors, and eventually control hardware — NEPTUNE is your local JARVIS in the making.

---

## ✅ What We Built

* ✅ **Flask backend server (`neptune.py`)** for OpenAI/Groq communication
* ✅ **Speech-to-text** using SpeechRecognition + PyAudio
* ✅ **Voice output** using pyttsx3 and ElevenLabs premium voice models
* ✅ **Mic-to-response bridge** (`bridge_neptune_voice_eleven.py`) for real-time flow
* ✅ Animated **dark-themed web UI** with glowing input, dropdown provider switch
* ✅ Built-in `/ask` endpoint for command handling
* ✅ App runs at `localhost:5000` with full CORS enabled
* ✅ Designed for automation add-ons like job form autofill, resume summarizing, and sensor input parsing

---

## ⚙️ Technologies Used

* Flask, Python 3.10, dotenv, requests, HTML/CSS/JavaScript
* SpeechRecognition, PyAudio
* pyttsx3 / ElevenLabs (TTS)
* Selenium + PyAutoGUI (job app automation)

---

## 🧠 How to Run NEPTUNE

```bash
# Step 1: Create and activate virtual environment
python3 -m venv neptune-venv
source neptune-venv/bin/activate

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Run the assistant
python3 neptune.py
```

🔑 Notes:

* Requires working mic permissions on Linux
* ElevenLabs API key required for premium voice
* Groq requires `choices` field in response JSON

📸 *Dark mode UI screenshots, glowing avatar states, and video demo in progress*

---

# 🏠 SmartPad – ESP32 Smart Home System

A full-featured smart home automation prototype using sensors, relays, and a custom web dashboard.

---

## ✅ What We Did

* ✅ Connected DHT11 sensor to display live temp & humidity
* ✅ Set up PIR sensor to detect motion and trigger alerts
* ✅ Linked buzzer to motion for sound alarm
* ✅ Controlled external device with relay (e.g., fan/lamp)
* ✅ Built and served responsive web dashboard via ESP32

---

## ⚙️ Tech Stack

* ESP32, DHT11, PIR Sensor, Relay Module, RGB LED
* HTML/CSS/JS dashboard served via ESPAsyncWebServer

📸 *Photos and video coming soon*

---

# 🐾 TouchPet – Tamagotchi-Style Virtual Pet Game

Touchscreen-based pixel pet game with mood and hunger tracking.

---

## ✅ What We Did

* ✅ Designed sprite faces for happy, sad, tired, and hungry moods
* ✅ Programmed button interface to feed, play, or rest your pet
* ✅ Displayed real-time status via OLED
* ✅ Used OOP in C++ to structure pet behavior logic

---

## ⚙️ Tech Stack

* ESP32, ILI9341 2.8" Touchscreen, TFT\_eSPI, TouchLib
* Object-oriented C++ game loop

📸 *Gameplay and sprite animation preview coming soon*

---

# 👁️ WatchCat – ESP32-CAM Motion Alert System

A mini surveillance system using ESP32-CAM and motion detection.

---

## ✅ What We Did

* ✅ Set up ESP32-CAM for live video stream
* ✅ Connected PIR sensor to detect motion
* ✅ Triggered visual LED alerts on motion
* ✅ Built test system for future cloud sync expansion

---

## ⚙️ Tech Stack

* ESP32-CAM, PIR sensor, LED output
* Arduino IDE with serial debugging

📸 *Video feed snapshot and alert demo coming soon*

---

# 🎛️ ControlBox v1 – Modular Sensor Panel

All-in-one dev rig with multiple inputs and outputs for sensor testing.

---

## ✅ What We Did

* ✅ Wired up joystick, buttons, and RFID module
* ✅ Added LCD1602 display for feedback
* ✅ Created flexible header system for swapping sensors
* ✅ Used for logic testing, I/O control, and classroom-style demos

---

## ⚙️ Tech Stack

* ESP32, MFRC522 RFID, LCD1602, Joystick, Buttons
* Wood panel mounted for portability

📸 *Photos of sensor panel and test outputs coming soon*

---

# 📚 DevBoard Library – Wiring + Codebase Templates

Collection of starter templates and wiring guides for rapid prototyping.

---

## ✅ What We Did

* ✅ Created reusable C++ functions for RGB, OLED, buzzer, etc.
* ✅ Made labeled diagrams for sensor pinouts
* ✅ Included example sketches for ultrasonic, temp/humidity, motion
* ✅ Added OTA example for updating firmware wirelessly

---

## ⚙️ Tech Stack

* ESP32, Breadboard, OLED SSD1306, DHT11, HC-SR04, RGB LED, Arduino IDE

📸 *Wiring diagrams and breadboard photos coming soon*

---

# 💬 Freelance Availability

I specialize in creating embedded systems and automation interfaces for personal, commercial, or educational use.

💼 **Services Offered**

* 🔧 Custom ESP32/Arduino device development
* 🖥️ UI dashboards (touchscreen or web-based)
* 🐞 Debugging and code refactoring
* 🔌 Breadboard prototyping and wiring documentation
* 📦 Project packaging and delivery-ready builds

📧 **Contact:** [mobileitsoulutions222@gmail.com](mailto:mobileitsoulutions222@gmail.com)

Let’s build something dope together 🚀
