Prototype of a Four Way Traffic Light Control System with 7-Segment Display. 

This project was designed as part of the requirements for completing the final year PLC programming course under the Mechatronics Elective of the Department of Mechanical Engineering at the Federal Univeristy of Technology Akure. Headed by Prof. O.A. Dahunsi.  

This project is designed to simulate a traffic light system for four directions and a 7-segment display to show a countdown timer using an Arduino. 

Project Overview 

The goal of this project is to control a set of traffic lights and a 7-segment display using an Arduino. The system will manage the traffic lights for all four directions, ensuring that cars move safely and efficiently. The 7-segment display will show a countdown timer, indicating how much time is left before the lights change. 

Features 

Traffic Lights Control: The system controls the green, yellow, and red lights for North, South, East, and West directions. 

Countdown Timer: A 7-segment display shows the remaining time before the lights change. 

Shift Registers: Efficient use of shift registers to control the LEDs and the seven-segment displays, freeing up GPIO pins on the Arduino. 

Components Used 

Arduino Uno  

LEDs (12 in total: 3 for each direction - red, yellow, and green) 

7-Segment Display 

2 X Shift Registers (74HC595) 

220 ohm Resistors 

Breadboard and Jumper Wires 

9V Battery 

Switch  

Copper Wire 

Software 

Embedded C 

 

 

How It Works 

The system operates in a loop, cycling through each direction and controlling the traffic lights accordingly. This cycle repeats indefinitely, ensuring safe and controlled traffic flow.  Here's a brief overview: 

Junction-1: The green light for this junction is on, allowing cars to move. The 7-segment display counts down from 9 to 0. 

Transition to Junction-2: Junction-1’s light turns yellow, preparing to stop cars. The countdown continues. 

Junction-2: The green light for this junction is on, allowing cars to move. The countdown resets and continues. 

Transition to junction-3: Junction-2’s light turns yellow, preparing to stop cars. The countdown continues. 

Junction-3: The green light for this junction is on, allowing cars to move. The countdown resets and continues. 

Transition to Junction-4: Junction 3’s light turns yellow, preparing to stop cars. The countdown continues. 

Junction-4: The green light for this junction is on, allowing cars to move. The countdown resets and continues. 

Transition to Junction-1: Junction-4’s light turns yellow, preparing to stop cars. The countdown continues. 

 
