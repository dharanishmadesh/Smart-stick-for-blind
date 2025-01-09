

# **Smart Stick for Blind People** 🚶‍♂️💡

This project is designed to help visually impaired people navigate their surroundings using a smart stick with ultrasonic sensors. The stick uses two ultrasonic sensors to measure the distance to obstacles and triggers a buzzer to alert the user if an object is too close. This system improves mobility and safety for blind and visually impaired individuals.

---

## **✨ Features**

- **Dual Ultrasonic Sensors**: Two ultrasonic sensors placed on the stick to detect objects from both the front and side, helping the user avoid obstacles.
- **Buzzer Alert**: The system emits a sound when an object is detected within a set range.
- **Simple and Cost-Effective**: Uses affordable and readily available components for ease of implementation and low cost.

---

## **📂 Folder Structure**

- `SmartStick.ino`  
  - Main Arduino sketch file for the Smart Stick system.
- `README.md`  
  - Documentation for the project.
- `LICENSE`  
  - Open-source license details (if applicable).

---

## **🔧 Hardware Components**

- **Arduino Board** (e.g., Arduino Uno or Nano)
- **2x Ultrasonic Sensors** (HC-SR04 or similar)
- **Buzzer**
- **Jumper wires**
- **Breadboard** (optional)
- **Power supply** (e.g., 9V battery or USB power)

---

## **🔌 Circuit Connections**

| Component                | Pin Assignment   |
|--------------------------|------------------|
| **Ultrasonic Sensor A**   | Trigger: A0, Echo: A1 |
| **Ultrasonic Sensor B**   | Trigger: A3, Echo: A2 |
| **Buzzer**                | Pin 2            |
| **Arduino Board**         | Power Pins       |

---

## **⚙️ Software Requirements**

- Arduino IDE (version 1.8.10 or later)

---

## **🚀 How to Use**

1. **Setup**  
   - Connect the two ultrasonic sensors and the buzzer to the Arduino as described in the circuit section.
   - Power the Arduino with a suitable power source (e.g., battery or USB).

2. **Upload Code**  
   - Open the `SmartStick.ino` file in Arduino IDE.
   - Select the correct board and port under **Tools**.
   - Upload the code to your Arduino board.

3. **Operation**  
   - The system continuously measures the distance to obstacles using the two ultrasonic sensors.
   - If an obstacle is detected within the set range, the buzzer will sound to alert the user.
   - If no obstacle is detected, the buzzer remains off, indicating a clear path.

---

## **💡 Code Overview**

The system works by using two ultrasonic sensors to measure the distance to obstacles in front and to the side of the user. If an object is detected within the set range (e.g., 10–200 cm), the buzzer is triggered:

```cpp
// Front Sensor
if (distance >= 10 && distance <= 200) {
  digitalWrite(BUZZER, LOW);  // No obstacle, buzzer off
} else {
  digitalWrite(BUZZER, HIGH); // Obstacle detected, buzzer on
}

// Side Sensor
if (bdistance >= 11 && bdistance <= 200) {
  digitalWrite(BUZZER, LOW);  // No obstacle, buzzer off
} else {
  digitalWrite(BUZZER, HIGH); // Obstacle detected, buzzer on
}
```

---

## **📜 License**

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---

## **🤝 Contributing**

Contributions are welcome! You can:
- Submit a pull request with new features or bug fixes.
- Open an issue to report bugs or suggest improvements.

---

## **💬 Feedback**

For questions, suggestions, or feedback, feel free to open an issue or contact me directly.

---

This project aims to make navigation easier for people with visual impairments, allowing them to move around safely and with confidence.

---

Stay Safe! 🚶‍♂️
