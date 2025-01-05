# Ultrasonic Sensor and Buzzer Project

## Overview
This project demonstrates the use of an ultrasonic sensor and a buzzer to create a distance-based alarm system. The buzzer sounds when an object is detected within a specified range (e.g., 50 cm) by the ultrasonic sensor.

## Components Required
- Arduino Uno
- Ultrasonic Sensor (e.g., HC-SR04)
- Buzzer
- Jumper Wires
- Breadboard
- 6 AA Battery Holder (9V) or equivalent power source

## Circuit Diagram
### Ultrasonic Sensor (HC-SR04):
- **VCC**: Connect to Arduino's 5V pin.
- **GND**: Connect to Arduino's GND pin.
- **Trigger Pin**: Connect to Arduino Digital Pin 11.
- **Echo Pin**: Connect to Arduino Digital Pin 12.

### Buzzer:
- **Positive Pin**: Connect to Arduino Digital Pin 3.
- **Negative Pin**: Connect to Arduino GND.

### Power Source:
- Connect the positive terminal of the battery holder to Arduino's Vin pin.
- Connect the negative terminal of the battery holder to Arduino's GND pin.

## Project Working
1. The ultrasonic sensor emits an ultrasonic pulse through its Trigger Pin.
2. The pulse travels through the air and reflects back upon hitting an object.
3. The reflected pulse is received by the sensor's Echo Pin.
4. The Arduino calculates the distance of the object using the time taken for the pulse to travel to the object and back.
5. If the distance is below a specified threshold (e.g., 5 cm), the buzzer is activated.
6. If the distance exceeds the threshold, the buzzer remains off.

## Connections Overview
### Ultrasonic Sensor:
- VCC to 5V
- GND to GND
- Trigger Pin to Digital Pin 11
- Echo Pin to Digital Pin 12

### Buzzer:
- Positive to Digital Pin 3
- Negative to GND

### Power Supply:
- Positive terminal of the battery to Vin
- Negative terminal of the battery to GND

## Features
- Distance-based alarm system.
- Portable design using a battery pack.
- Easily adjustable distance threshold (by modifying the code).
- Can be used in various applications like proximity alarms, parking assistance, etc.

## Applications
- Security systems
- Obstacle detection in robotics
- Parking assistance systems
- Proximity alarms
