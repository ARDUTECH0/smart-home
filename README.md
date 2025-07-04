<h1 align="center">🔌 ATWALLX</h1>

A professional, feature-rich firmware for smart relay systems built on **ESP8266 / ESP32 / ESP8285**, designed to deliver seamless control, automation, and real-time monitoring for smart home and industrial applications.

## ✨ Key Features

| Icon | Feature | What it means for you |
| ---- | ------- | --------------------- |
| 🕒 | **Weekly Scheduler** | Plan automatic ON/OFF times for every day of the week—no need to remember manual switches. |
| ⏳ | **Delayed Actions** | Tap once, and the relay will turn ON or OFF after the delay you choose. Perfect for stair‑well lights or fans. |
| 🧲 | **Sensor‑Triggered Switching** | Attach motion, light, or temperature sensors and let the system react instantly—hands‑free. |
| 🧠 | **EEPROM State Memory** | Even after a power cut, the last relay states are safely restored when power returns. |
| 📶 | **OTA Updates** | Get the latest firmware in one click—no cables or dismantling. |
| 🎙️ | **Google Voice Control** | Say “Hey Google, turn on the …” and the relay obeys. Voice commands also work directly inside the mobile app. |

---

### 📱 Get the App

1. **Download:** [Android inks go here]  
2. **Pair:** Connect to your Wi‑Fi and scan for devices.  
3. **Control:** Use taps, schedules, sensors, *or your voice*—all in one place.

> **Tip:** Make sure your phone and the device are on the same network the first time you pair them.


| Platform | Link |
|----------|------|
| 📱 Android | [Download](https://github.com/ARDUTECH0/smart-home/raw/refs/heads/main/app-release.apk) |


> 🔑 Requires device to be connected to Wi-Fi .

---

## 🧮 Relay & Button Pin Mapping

| Relay Index | Relay Pin | Button Pin |
|-------------|-----------|------------|
| 0           | D0        | D2         |
| 1           | D1        | D4         |

> You can press each button to toggle the corresponding relay manually. Button logic includes debounce handling.

---
## 📥 Download Binary Firmware

> Choose the right firmware for your board and flash it using the method below:

| Platform | Firmware Link |
|----------|----------------|
| ESP8266  | [Download ESP8266 Firmware](https://github.com/ARDUTECH0/smart-home/raw/refs/heads/main/Firmware_1.5V.bin) |

---

## 🚀 Flashing the Firmware

### 1. Using ESPHome-Flasher (GUI)
- Download `.bin` file
- Connect your board via USB
- Select COM Port and `.bin` file
- Click **Flash**
---

## 🔄 Flash Firmware via Web Installer

You can easily upload the firmware to your ESP8266 / ESP32 device using a web browser — no need for extra tools!

### 🌐 Online Flasher:
> [https://esp.huhn.me](https://esp.huhn.me)

### 🧭 How to Use:

1. Visit **[esp.huhn.me](https://esp.huhn.me)** using **Google Chrome** or **Microsoft Edge**.
2. Connect your ESP device via **USB** to your computer.
3. Click "**Connect**" and select your device's COM port.
4. Choose the firmware `.bin` file from your computer.
5. Flash and wait until the process is complete.

> ⚠️ **Note:** This only works over USB

### 2. Using `esptool.py` (CLI)
```bash
# ESP8266
esptool.py --port COM3 write_flash 0x0 firmware_esp8266.bin

# ESP32
esptool.py --chip esp32 --port COM3 write_flash -z 0x1000 firmware_esp32.bin
```
---

## 📲 Adding the Device via the Mobile App

To add your Smart Relay device using the mobile app, follow these steps **carefully**:

1. **Connect your phone** to the Wi-Fi network created by the device:  
   > 📶 SSID format: `ATWALLX_XXXXXX`

2. Open the **ATWALLX**.

3. Tap the ➕ icon at the top to **add a new device**.

4. Once detected, the app will show a screen to enter your **home Wi-Fi credentials** (SSID & Password).

5. Tap **Save** and wait while the device reboots and connects to your router.

> ⚠️ **Important:** You must be connected to the device’s Wi-Fi (ATWALLX_XXXXXX) during this step, or the app won’t detect the device.
---
## 📞 Contact & Support

Need help or have a custom integration request?

Feel free to contact us:

- 💬 WhatsApp: [+201096448029](https://wa.me/201096448029)

We're happy to help with:
- Integration support
- Feature requests
- Custom firmware
- Commercial deployments

