# **Prototype of a Four Way Traffic Light Control System with 7-Segment Display**

This project was designed as part of the requirements for completing the final year PLC programming course under the Mechatronics Elective of the Department of Mechanical Engineering at the Federal University of Technology Akure. Headed by Prof. O.A. Dahunsi.

This project is designed to simulate a traffic light system for four directions and a 7-segment display to show a countdown timer using an Arduino.

## **Project Overview**

The goal of this project is to control a set of traffic lights and a 7-segment display using an Arduino. The system will manage the traffic lights for all four directions, ensuring that cars move safely and efficiently. The 7-segment display will show a countdown timer, indicating how much time is left before the lights change.

## **Features**

- **Traffic Lights Control**: The system controls the green, yellow, and red lights for North, South, East, and West directions.
- **Countdown Timer**: A 7-segment display shows the remaining time before the lights change.
- **Shift Registers**: Efficient use of shift registers to control the LEDs and the seven-segment displays, freeing up GPIO pins on the Arduino.

## **Components Used**

- Arduino Uno
- LEDs (12 in total: 3 for each direction - red, yellow, and green)
- 7-Segment Display
- 2 X Shift Registers (74HC595)
- 220 ohm Resistors
- Breadboard and Jumper Wires
- 9V Battery
- Switch
- Copper Wire

## **Software**

- Embedded C

## **How It Works**

The system operates in a loop, cycling through each direction and controlling the traffic lights accordingly. This cycle repeats indefinitely, ensuring safe and controlled traffic flow. Here's a brief overview:

### **Junction-1 (South Direction):**
- **Green Light ON**: Cars at Junction-1 can move.
- **7-Segment Display**: The display shows a countdown starting from 9 down to 0, indicating the time left for cars to move.

### **Transition to Junction-2:**
- **Yellow Light ON**: Junction-1’s light turns yellow, signaling cars to prepare to stop.
- **Countdown Continues**: The 7-segment display continues counting down to 0.

### **Junction-2 (North Direction):**
- **Green Light ON**: Now, cars at Junction-2 can move.
- **Countdown Resets**: The 7-segment display resets to 9 and starts counting down again.

### **Transition to Junction-3:**
- **Yellow Light ON**: Junction-2’s light turns yellow, signaling cars to prepare to stop.
- **Countdown Continues**: The 7-segment display continues counting down to 0.

### **Junction-3 (East Direction):**
- **Green Light ON**: Cars at Junction-3 can move.
- **Countdown Resets**: The 7-segment display resets to 9 and starts counting down again.

### **Transition to Junction-4:**
- **Yellow Light ON**: Junction-3’s light turns yellow, signaling cars to prepare to stop.
- **Countdown Continues**: The 7-segment display continues counting down to 0.

### **Junction-4 (West Direction):**
- **Green Light ON**: Cars at Junction-4 can move.
- **Countdown Resets**: The 7-segment display resets to 9 and starts counting down again.

### **Transition Back to Junction-1:**
- **Yellow Light ON**: Junction-4’s light turns yellow, signaling cars to prepare to stop.
- **Countdown Continues**: The 7-segment display continues counting down to 0.
