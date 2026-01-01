# arduino-line-follower-robot
An Arduino-based autonomous line follower robot using IR sensors for real-time path detection and motor control.

# Line Follower Robot using Arduino 

An autonomous **Line Follower Robot** built using **Arduino**, **IR sensors**, and a **motor driver**.  
The robot detects a black line on a white surface and follows it automatically based on sensor feedback.

---

##  Project Overview

The Line Follower Robot uses **two IR sensor modules** (left and right) to detect a black line.  
The sensor data is processed by the Arduino, which controls the motors through a motor driver to keep the robot aligned with the path.

---

##  Hardware Requirements

- Arduino Uno / Nano  
- IR Sensor Module × 2  
- L298N / L293D Motor Driver  
- DC Gear Motors × 2  
- Robot Chassis  
- Wheels × 2  
- Castor Wheel  
- Battery (7V–12V)  
- Jumper Wires  

---

## 🔌 Pin Configuration

### IR Sensors
| Sensor | Arduino Pin |
|------|-------------|
| Left IR Sensor | D2 |
| Right IR Sensor | D3 |

### Motor Driver
| Motor Driver Pin | Arduino Pin |
|----------------|------------|
| IN1 | D5 |
| IN2 | D6 |
| IN3 | D9 |
| IN4 | D10 |
| ENA | D7 |
| ENB | D8 |

---

##  Working Principle

The IR sensors detect whether the surface beneath them is **black or white**.

| Left Sensor | Right Sensor | Action |
|-----------|-------------|--------|
| Black | Black | Move Forward |
| Black | White | Turn Left |
| White | Black | Turn Right |
| White | White | Stop |

> **Note:**  
- Black line → `LOW`  
- White surface → `HIGH`

---


