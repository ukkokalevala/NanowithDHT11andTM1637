1. Hardware Requirements

    Arduino Nano
    DHT11 temperature and humidity sensor
    TM1637 4-digit 7-segment display
    Breadboard and jumper wires

Wiring Diagram
DHT11 Sensor

    VCC to 5V
    GND to GND

    Data to Digital Pin 2 (with a 10k pull-up resistor)

TM1637 Display

    VCC to 5V
    GND to GND
    CLK to Digital Pin 3
    DIO to Digital Pin 4

Arduino Code

First, install the necessary libraries:

    DHT sensor library by Adafruit
    TM1637Display library

You can install these libraries through the Arduino IDE Library Manager.
Libraries: The code includes the Adafruit DHT and TM1637Display libraries to interact with the DHT11 sensor and the TM1637 display.
Pin Definitions: The DHT11 data pin is connected to digital pin 2, and the TM1637 display uses digital pins 3 (CLK) and 4 (DIO).
Setup: The setup() function initializes the serial communication, DHT sensor, and TM1637 display.
Loop: The loop() function reads temperature and humidity from the DHT11 sensor and displays the temperature on the TM1637 display. It also prints a message if the sensor read fails.
