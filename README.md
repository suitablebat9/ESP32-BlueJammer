# ESP32-BlueJammer

# ESP32-BlueJammer

**Bluetooth/BLE/WiFi/2.4GHz Jamming Board**

The **ESP32-BlueJammer** is a compact, feature-packed board designed to disrupt devices operating in the 2.4GHz frequency range using ESP32 and nRF24 modules. It generates noise and excessive packets (DoS) that interfere with:

- Bluetooth audio and data connections
- WiFi networks
- BLE devices
- RC drones
- IoT devices

> ⚠️ **Disclaimer:** This project is based on the work of [Emensta](https://github.com/Emensta). I only created the PCB to make the project easier to use. All original credit goes to them.

---

## 🔧 Features

- Toggle power with a built-in switch
- Momentary activation with onboard button
- Solder pads labeled `EXT Switch` for external/wireless activation
- `EXT Power` pads for external 5V power input (Left = GND, Right = 5V)
- Combo firmware support – change modes via ESP32 boot button
- Blue status LED (can be disabled with jumper)
- PH 2.0 battery connector (battery not included, connector provided)
- USB Type-C power input (not the ESP32 USB)

---

## 🔌 Mode Descriptions

| Mode | Description | Frequency Range |
|------|-------------|-----------------|
| BT 80CH | Classic Bluetooth Jammer | 2.402 GHz – 2.480 GHz |
| BLE 40CH | Bluetooth Low Energy Jammer | 2.400 GHz – 2.4835 GHz |
| BT-BLE 40-80CH | BT + BLE Jammer | 2.400 GHz – 2.4835 GHz |
| BT-WiFi 14-80CH | BT + WiFi Jammer | 2.400 GHz – 2.4835 GHz |
| WiFi 14CH | WiFi Jammer | 2.400 GHz – 2.4835 GHz |
| 2.4GHz All 1-125CH | RC Drone Jammer | 2.400 GHz – 2.525 GHz |

The current mode is shown via the **blue jamming LED**, based on a blinking pattern. Refer to the **LED key printed on the PCB**.

---

## 📂 Files Included

- `schematic/` – PDF schematic of the board
- `firmware/` – Instructions or link to Emensta's original firmware
- `board/` – Gerber files for manufacturing
- `images/` – Photos and board reference images
- `customization/` – Optional user modifications

---

## 🔒 Legal Disclaimer

Please use this tool responsibly and only in controlled environments with devices you own. **Do not use this against others without explicit permission.** Check your country's regulations before operating jamming devices.

> I am not responsible for any misuse of this board.

---

## 📬 Custom Orders

Want the ESP32 or NRF24 module **soldered directly** instead of using sockets? Leave a message with your order number.

---

## 📷 Images

(Add pictures in the `images/` folder and reference them here using markdown.)

```markdown
![Top View](images/top.jpg)
![Back View](images/back.jpg)
