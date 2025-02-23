"# automatedplantwateringsystem" 
# Automated Plant Watering System

An automated plant watering system using Arduino that monitors soil moisture levels and controls water flow using a relay. The system displays real-time soil status on an LCD screen and automates watering, ensuring efficient water usage and reducing manual intervention.

## 🚀 Features

- Real-time soil moisture monitoring using a soil moisture sensor.
- Automated control of the water pump based on moisture levels.
- LCD display for live soil moisture status and motor control updates.
- Reduces water wastage by watering only when the soil is dry.
- Serial monitor feedback for debugging and data logging.

## 🔧 Technologies & Components Used

- **Arduino Uno**  
- **Soil Moisture Sensor**  
- **Relay Module**  
- **LiquidCrystal I2C (16x2 LCD Display)**  
- **C++ (Arduino IDE)**  
- **IoT Integration (Optional for Remote Monitoring)**  

## 💡 How It Works

1. The soil moisture sensor reads the moisture level of the soil.  
2. The LCD displays the current soil status:
   - **Soil Dry**: Turns the motor **ON** to water the plant.  
   - **Soil Medium**: Turns the motor **OFF**, as moderate moisture is detected.  
   - **Soil Wet**: Keeps the motor **OFF** when adequate moisture is present.  
3. The relay module controls the motor based on the sensor data, ensuring precise watering.

## 🛠️ Circuit Connections

| **Component**           | **Arduino Pin** |
|-------------------------|------------------|
| Soil Moisture Sensor    | A0               |
| Relay Module (Motor)    | 7                |
| I2C LCD SDA             | A4               |
| I2C LCD SCL             | A5               |
| VCC & GND               | 5V & GND         |

## ⚡ Code Overview

- **Reading Sensor Data:**  
  The `analogRead()` function reads moisture levels from the sensor.  
- **Controlling Motor:**  
  The relay is triggered to turn the motor ON/OFF based on threshold values.  
- **Displaying Status:**  
  The LCD shows live updates on soil conditions and motor state.

## 🏃 Getting Started

### Prerequisites
- **Arduino IDE** installed on your computer.
- Install the `LiquidCrystal_I2C` library from the Arduino Library Manager.

### Uploading the Code
1. Connect the Arduino to your PC via USB.
2. Open the Arduino IDE and paste the provided code.
3. Select the appropriate port and board (Arduino Uno).
4. Click on **Upload**.

## 🌿 Output Example


The LCD will display corresponding messages, and the motor will activate or deactivate accordingly.

## 💬 Future Improvements

- Add IoT capabilities for remote monitoring and scheduling.
- Implement mobile notifications when soil moisture is low.
- Optimize the watering algorithm based on plant types and weather conditions.

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or pull requests for enhancements.

---

📫 **Contact:** [Your Email/Portfolio Link]  
🌟 *If you found this project useful, give it a star!*
