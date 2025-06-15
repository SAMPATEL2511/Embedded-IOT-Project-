# Embedded-IOT-Project-
A Bluetooth-controlled mini elevator system using Arduino, designed for IoT and embedded systems coursework.


# 🚀 Bluetooth-Controlled Mini Elevator System

A Bluetooth-controlled miniature elevator system designed and built as part of the **Internet of Things (IoT) and Embedded Systems** course at Università di Roma, 2023–2024. This system mimics a standard elevator using Arduino, motor control, and wireless communication with an Android device.

---

## 📌 Project Overview

This project showcases the integration of mechanical design, embedded programming, and Bluetooth communication to build a functional, scaled-down elevator system. It simulates real-world elevator operations, complete with acceleration, deceleration, and floor selection using a mobile app.

---

## 🛠️ Features

- Three-floor elevator system
- Bluetooth-based control using a custom Android app
- Ultrasonic distance sensing for floor detection
- Limit switches for safety bounds
- Arduino-based PWM motor control
- Smooth dynamic behavior (acceleration/deceleration)
- Real-time feedback loop to manage errors and noise

---

## 🧰 Hardware Components

| Component                  | Purpose                                             |
|---------------------------|-----------------------------------------------------|
| Arduino UNO               | Main microcontroller                                |
| HC-SR04 Ultrasonic Sensor | Measures carriage position                          |
| 30V DC Motor              | Elevator prime mover                                |
| L298N Motor Driver        | Motor control and speed direction                   |
| HC-05 Bluetooth Module    | Wireless communication with Android device          |
| Limit Switches            | Floor detection and stopping mechanism              |
| Wooden Frame              | Physical structure for elevator support             |
| Pulley & Belt System      | Mechanical motion control                           |

---

## 📐 Mechanical Design

- Frame Dimensions: `200mm x 300mm x 1300mm`
- Carriage constrained in Z-direction
- Belt-driven movement via motor and pulley
- Handcrafted components for prototyping

---

## ⚡ Electrical Design

- Power: 24V DC supply for motor, 9V for Arduino
- Tachometer feedback through analog input
- PWM used for speed control (10-bit resolution)
- Full circuit diagrams included in the PDF documentation

---

## 💡 Control & Programming

- Written in C++ for Arduino using GyverMotor and ezButton libraries
- Core functions: `goUp()`, `goDown()`, `stop()`, `goHome()`
- Limit switch debounce for safety
- Real-time distance calculation from ultrasonic sensor
- Bluetooth commands: `'+'` (start), `'-'` (stop), `'0'`, `'1'`, `'2'` for floors

---

## 📱 Mobile App Interface

- Built with [MIT App Inventor](https://appinventor.mit.edu/)
- Connects to Arduino via Bluetooth
- Simple interface with:
  - List Picker for Bluetooth connection
  - Toggle switch to turn elevator ON/OFF
  - Floor selection buttons (Ground, 1st, 2nd)

---

## 📊 Results

- Smooth motion verified
- Real-time Bluetooth control from Android phone
- Low noise and effective feedback handling
- Successfully handled system disturbances (dead weight, friction)

---

## ✅ Conclusions

This mini elevator system effectively simulates real elevator dynamics. It validates core IoT and embedded systems concepts like sensor feedback, motor control, and mobile integration.

---

## 📄 References

1. Giancarlo Orengo – Lesson Notes “Prototyping Boards & Languages for IoT”
2. M. Margolis – Arduino Cookbook, 2nd Ed.
3. RS PRO Datasheet – 30W Servo Motor (DC 24–30V, 1600 rpm)

---

## 📃 License

This project is open for academic and prototyping use. Consider adding a `LICENSE` file for proper attribution.

---

## 📎 Acknowledgements

Developed by **Parth Bhalani**  
Course: *Electronic IoT and Embedded Systems (EIES)*  
Supervisor: Prof. **Giancarlo Orengo**, Università di Roma  
