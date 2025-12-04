# HOME-AUTOMATION-5C-PCB

# Smart Home Automation PCB

This is an open-source ESP32-based smart home automation PCB designed by me.  
It includes zero-cross detection, triac dimming, relay control and support for Alexa/Google integration (optional).

---

## 🚀 Features
- ESP32-based main controller  
- 4N25 Zero-Cross Detection  
- Triac-based AC dimming  
- Relay output for AC load ON/OFF  
- Indicator LEDs  
- Safe opto-isolated design  
- Can be used for fan dimming & bulb control  

---

## 🧰 Files in this Repository
- `schematics/` → Circuit diagram  
- `pcb/` → PCB design files  
- `firmware/` → ESP32 code  
- `bom/` → Part list of components  
- `images/` → PCB photos & renders  

---

## 🔧 How to Use / Instructions

### 1) Assemble the PCB
- Solder all resistors  
- Solder optocouplers (4N25, MOC3021, etc)  
- Solder triac (BT136 or chosen model)  
- Mount terminal blocks  
- Insert ESP32  

### 2) Power Requirements
- 5V input via Hi-Link / External SMPS  
- ESP32 runs at 3.3V (regulator included)

### 3) Upload the Firmware
1. Download code from `firmware/` folder  
2. Open in Arduino IDE or PlatformIO  
3. Select board → ESP32 Dev Module  
4. Upload code  
5. Open Serial Monitor → you should see boot messages  

### 4) Connecting AC Load (⚠️ Safety First!)
- Only connect AC when you are confident  
- Use proper insulation  
- Fan/Bulb should connect through triac output  
- Relay output supports ON/OFF loads  

---

## 🧪 Testing
- Connect a test load or bulb  
- Verify Zero-Cross is detected (LED should blink)  
- Check dimming using serial or app  
- Test safety circuits  

---

## 🤝 Contributing
If you want to improve this project:
- Open an issue  
- Submit a pull request  
- Suggest new features  

---

## 📜 License
This project is open-source under the MIT License.

---

## 📞 Contact
Maintainer: **Govind**  
GitHub: https://github.com/govindverma04
