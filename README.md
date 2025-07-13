# Arduino Robot 🤖

An intelligent, Arduino-based robotic system designed to navigate environments autonomously using Arduino Uno, Ultrasonic Sensor (HC-SR04), DC Motors, and a Servo Motor. This system detects obstacles and moves seamlessly in dynamic environments.

<table> <tr>  <td><img src="https://i.ibb.co/1GG0J9sS/Whats-App-Image-2025-07-12-at-01-51-57-27c76680.jpg" alt="image1" height="500"/></td>  <td><img src="https://i.ibb.co/KpCnyp9F/Whats-App-Image-2025-07-12-at-01-51-58-c9064daa.jpg" alt="image2" height="500"/></td></td> </tr>  </table>

---

## 🌟 Key Features

* **Autonomous Navigation:** Uses an ultrasonic sensor to detect obstacles and adjust its path.
* **Real-Time Feedback:** Can be configured to display status updates (e.g., "Moving Forward" or "Obstacle Detected") with an optional LCD.
* **Dynamic Movement:** Controls two DC motors for wheel movement and a servo for additional functionality.
* **Customizable Behavior:** Allows adjustments to sensor range and motor settings.

---

## 🔧 Components Used

| Component                     | Functionality                                                 |
| :---------------------------- | :------------------------------------------------------------ |
| **Arduino Uno** | Microcontroller for processing sensor inputs and controlling motors. |
| **Ultrasonic Sensor (HC-SR04)** | Detects obstacles by measuring distances in the robot’s path. |
| **DC Motors (x2)** | Drives the robot’s wheels for forward, backward, and turning movements. |
| **Servo Motor** | Provides additional movement control (e.g., steering or arm). |
| **Motor Driver Shield** | Interfaces Arduino with motors, managing power and control signals. |
| **Power Supply** | 7.4-9V battery pack to power the motors and shield.           |

---

## ⚙️ System Workflow

1. **Obstacle Detection**
   - **Ultrasonic Sensor (HC-SR04):** Measures distance to objects in front of the robot.
   - **Action:**
     - If the path is clear → Robot moves forward  
     - If an obstacle is detected → Robot stops or turns based on programmed logic

2. **Movement Control**
   - **DC Motors:** Controlled via the **Motor Driver Shield** to enable navigation.  
   - **Servo Motor:** Used for additional movements, adjustable via the shield.

3. **Power Management**
   - **7.4–9V Battery:** Supplies power to the **Motor Driver Shield**, which distributes it to motors and sensors.

---

## 🚀 Getting Started

### 1. Prerequisites

#### Hardware
- Arduino Uno  
- Ultrasonic Sensor (HC-SR04)  
- 2 DC Motors  
- Servo Motor  
- Motor Driver Shield (compatible with Arduino)  
- 7.4–9V Battery Pack  
- Jumper Wires  
- Breadboard (optional)  

#### Software
- Arduino IDE  

---

### 2. Setup

#### 1. Clone the Repository
```bash
git clone https://github.com/Arduino_Robot
```

### 2. Upload Code

- Open the Arduino IDE.  
- Connect your Arduino Uno via USB.  
- Upload the provided sketch (`Arduino_Robot.ino`) to the board.

### 3. Assemble Hardware

- Connect the ultrasonic sensor, DC motors, servo motor, and battery to the Motor Driver Shield as per the circuit diagram.  
- Ensure correct pin assignments (e.g., Trig and Echo for the sensor).

### 4. Power the System

- Attach the 7.4–9V battery to the shield.  
- Test the robot in an open area with obstacles.

---

## 📋 Technical Specifications

* **Detection Range:** Up to 4 meters with HC-SR04 (adjustable in code).
* **Power Supply:** 7.4-9V battery for motors, 5V from Arduino for sensors.
* **Motor Control:** Managed via Motor Driver Shield with precise speed and direction.

---

## 🖼️ Visual Overview

### 1. Circuit Diagram
![Circuit Diagram](https://i.ibb.co/xtN3pn5N/arduino-obstacle-robot.jpg)

---

## 💡 Customization Options

* **Adjust Detection Range:** Modify the `MAX_DISTANCE` variable in the Arduino code.
* **Motor Speed Control:** Adjust PWM values in the code for motor speed.
* **Expand Functionality:** Add an LCD for status display or integrate Bluetooth for remote control.

---

## 📜 License

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it as needed.
