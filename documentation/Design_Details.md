# Design Details

## Step-by-Step Connections

### LEDs

#### South Direction LEDs:
- **SGreen (Pin 0)**: Connect to a green LED through a 220 ohm resistor.
- **SYellow (Pin 1)**: Connect to a yellow LED through a 220 ohm resistor.
- **SRed (Pin 2)**: Connect to a red LED through a 220 ohm resistor.

#### North Direction LEDs:
- **NGreen (Pin 3)**: Connect to a green LED through a 220 ohm resistor.
- **NYellow (Pin 4)**: Connect to a yellow LED through a 220 ohm resistor.
- **NRed (Pin 5)**: Connect to a red LED through a 220 ohm resistor.

#### East Direction LEDs:
- **EGreen (Pin 6)**: Connect to a green LED through a 220 ohm resistor.
- **EYellow (Pin 7)**: Connect to a yellow LED through a 220 ohm resistor.
- **ERed (Pin 8)**: Connect to a red LED through a 220 ohm resistor.

#### West Direction LEDs:
- **WGreen (Pin 9)**: Connect to a green LED through a 220 ohm resistor.
- **WYellow (Pin 10)**: Connect to a yellow LED through a 220 ohm resistor.
- **WRed (Pin 11)**: Connect to a red LED through a 220 ohm resistor.

### Shift Registers (74HC595)
- Connect the Vcc pin of both shift registers to the 5V pin of the Arduino.
- Connect the GND pin of both shift registers to the GND pin of the Arduino.
- Connect the SER (Serial Data Input) pin of the first shift register to the Arduino pin 12.
- Connect the SRCLK (Shift Register Clock Input) pin of the first shift register to the Arduino pin 13.
- Connect the RCLK (Register Clock/Latch Input) pin of the first shift register to the Arduino pin 10.
- Connect the Q7' (Serial Data Output) pin of the first shift register to the SER pin of the second shift register.
- Connect the SRCLK and RCLK pins of the second shift register to the same pins on the Arduino as the first shift register (pin 13 and pin 10, respectively).

### 7-Segment Display
- **Common Cathode/Anode**: Connect the common pin of the 7-segment display to the GND or Vcc, depending on the type (common cathode or anode).
- **Segments (A-G)**:
  - A (Pin A5)
  - B (Pin A4)
  - C (Pin A3)
  - D (Pin A2)
  - E (Pin A1)
  - F (Pin A0)
  - G (Pin 12)

### Power Supply
- Connect the 9V battery to the Arduino power jack or the Vin and GND pins.
- Add a switch between the battery and the Arduino to control the power.

## Circuit Diagram
Here’s a textual representation of how you would connect the components. For a visual representation, you can use Fritzing or any circuit diagram tool to draw it out.

## Putting It All Together
- Place all components on the breadboard.
- Connect the LEDs as described.
- Connect the shift registers to the Arduino and the 7-segment display.
- Connect the power supply.

By following these steps, the circuit for the traffic light control system with a 7-segment display using an Arduino and shift registers was set up.
