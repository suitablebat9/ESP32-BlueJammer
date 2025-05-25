# ESP32-BlueJammer

**Bluetooth / BLE / WiFi / 2.4GHz Jamming Board**

The **ESP32-BlueJammer** is a compact, feature-rich board designed to disrupt devices operating on the 2.4GHz frequency band. Powered by an ESP32 and an nRF24 module, it generates noise and sends excessive packets to interfere with:

- Bluetooth audio and data connections  
- WiFi networks  
- BLE (Bluetooth Low Energy) devices  
- RC drones and remotes  
- IoT gadgets and more

> ⚠️ **Disclaimer:** This project is based entirely on the work of [Emensta](https://github.com/EmenstaNougat/ESP32-BlueJammer). I created this PCB to make their project more plug-and-play. All credit for the original firmware and research goes to them.

---

## 🔧 Features

- Toggleable on/off switch  
- Onboard momentary activation button  
- **`EXT Switch`** solder pads for external or wireless switch activation  
- **`EXT Power`** solder pads for external 5V power input  
  - (Polarity: **Left = GND**, **Right = 5V** with antennas facing away from you)  
- Combo firmware support – press the ESP32’s boot button while powered to cycle modes  
- **Blue jamming LED** shows active mode (can be disabled via jumper)  
- PH 2.0 battery connector (battery not included, connector provided)  
- USB Type-C power input on the board (not on the ESP32 directly)

---

## 🔄 LED Blink Mode Key

The **blue jamming LED** will blink to indicate the current active jamming mode on combo firmware:

- `1 blink` = **BT** (Bluetooth Classic)  
- `2 blinks` = **BLE** (Bluetooth Low Energy)  
- `3 blinks` = **WiFi**  
- `4 blinks` = **RC** (2.4GHz Drone/Remote)

The blink key is also printed on the right side of the board for quick reference.

---

## 🛰️ Mode Descriptions

| Mode               | Description                         | Frequency Range          |
|--------------------|-------------------------------------|--------------------------|
| **BT 80CH**        | Bluetooth Classic Jammer            | 2.402 – 2.480 GHz        |
| **BLE 40CH**       | Bluetooth Low Energy Jammer         | 2.400 – 2.4835 GHz       |
| **BT-BLE 40-80CH** | Classic BT + BLE Combo Jammer       | 2.400 – 2.4835 GHz       |
| **BT-WiFi 14-80CH**| Classic BT + WiFi Combo Jammer      | 2.400 – 2.4835 GHz       |
| **WiFi 14CH**      | WiFi Jammer                         | 2.400 – 2.4835 GHz       |
| **2.4GHz All**     | RC / Drone Jammer (CH 1–125)        | 2.400 – 2.525 GHz        |

---

## 🔌 Flashing the Firmware

You can easily flash your board using the browser-based [ESP32 BlueJammer Web Flasher](https://esp32-bluejammerflasher.pages.dev/) provided by Emensta.

### Steps:
1. Visit [ESP32-BlueJammerFlasher](https://esp32-bluejammerflasher.pages.dev/)
2. Choose the firmware type, "Generic"
3. Choose the firmware you want to flash
4. Connect your ESP32 via a data USB cable
5. Flash the firmware of your choice

> 💡 Tip: If flashing fails, make sure you’re using a data-capable USB cable and have the correct drivers installed for your ESP32.

---

## 🛒 Buy the Board

Want a fully assembled board? You can purchase one from my Tindie store here:  
👉 [PCB Studios on Tindie](https://www.tindie.com/stores/pcb-studios/)

---

## 📦 What's Included

- Fully assembled **ESP32-BlueJammer PCB**
- PH 2.0 battery connector pre-installed
- Matching PH 2.0 connector for your battery (DIY soldering)
- Gerber files and schematic PDF (in this repo)

---

## ⚠️ Legal Notice

This project is for educational purposes only. Do not use this board to interfere with any wireless communications unless you have permission and are operating in a controlled, legal environment. You are solely responsible for what you do with this device.
