CONTACTLESS IR TEMPERATURE SENSOR

📌 Overview

This project is an Arduino-based smart alert system that detects nearby objects and measures their temperature using an ultrasonic sensor and an MLX90614 infrared temperature sensor.

If an object is detected within a certain distance and its temperature exceeds a predefined threshold, a buzzer alert is triggered. This system enables contactless temperature monitoring and can be used in safety and automation applications.

⚙️ Features
Contactless temperature sensing
Proximity-based activation
Real-time monitoring via serial output
Low-cost and easy-to-build hardware setup
🔌 Hardware Required
Arduino Uno/Nano
HC-SR04 Ultrasonic Sensor
MLX90614 Infrared Temperature Sensor
Buzzer
Jumper wires and breadboard
🔧 Pin Configuration

TRIG → D2
ECHO → D3
BUZZER → D5
MLX90614 → I2C (SDA, SCL)

📦 Libraries Required
NewPing
Adafruit MLX90614
Wire (pre-installed in Arduino IDE)
🚀 Working Principle

The system continuously measures the distance using the ultrasonic sensor.

When an object is detected within 10 cm, the MLX90614 sensor measures its temperature.

If the temperature exceeds 28°C, the buzzer is activated with rapid beeping.

If the temperature is below the threshold, no alert is triggered.

If no object is detected nearby, the system remains idle.

📊 Output Example

Distance: 8 cm | Temperature: 30.5 °C

🛠️ Future Improvements
Integration with LCD or OLED display
IoT-based remote monitoring using WiFi modules
Data logging and analytics
Visual indicators using LEDs
