# :ocean: Water Quality Monitoring System

An **Arduino-based Water Quality Monitoring System** that measures **TDS (Total Dissolved Solids), Conductivity, Salinity, and Temperature** to determine if water is safe for drinking.

## ⭐ Features
- ✅ **TDS Measurement** – Evaluates water purity  
- ✅ **Temperature Sensor** – Reads water temperature using DS18B20  
- ✅ **Salinity & Conductivity** – Estimates water properties  
- ✅ **Drinking Water Status** – Classifies water as drinkable or non-drinkable  

## 🛠 Hardware Requirements
- **Arduino Board** (Uno, Mega, etc.)
- **Gravity TDS Sensor**
- **DS18B20 Temperature Sensor** (with 4.7kΩ pull-up resistor)
- **LCD Display** (Optional, for on-device data display)
- **Jumper Wires & Breadboard**
- **Power Supply**

## 🏗 Circuit Diagram
Below is the wiring diagram for the project:

![Wiring Diagram](docs/wiring_diagram.png)

Ensure all connections are secure before powering the system.

## 🚀 Installation & Usage
### Clone the repository
```sh
git clone https://github.com/yourusername/WaterQualityMonitor.git
```
### Open the Arduino IDE and load the sketch
1. **Install required libraries**:
   - `DallasTemperature` (for DS18B20 sensor)
   - `EEPROM` (for data storage)
2. **Upload the code** to your Arduino board.
3. **Open the Serial Monitor (115200 baud rate)** to view real-time readings.

## 📊 How It Works
- The system reads **temperature** and **TDS** sensor values.
- It compensates TDS values based on temperature.
- Conductivity and salinity are estimated.
- The results are printed via the **Serial Monitor**.

## ⚠️ Water Quality Classification
| TDS Value (ppm) | Drinking Status        |
|-----------------|------------------------|
| `< 1000`       | ✅ Safe for drinking (Freshwater) |
| `> 1000`       | ❌ Not drinkable (Likely saltwater) |

## 🔧 Future Improvements
- Add **pH Sensor** support.
- Implement **Wi-Fi (ESP8266/ESP32) for remote monitoring**.
- Display results on an **LCD screen**.

## 📜 License
This project is open-source under the **MIT License**.

---

### 🤝 Contribute
Feel free to submit **issues, feature requests, or pull requests** if you’d like to contribute to this project.



