Password-Based Gate Control System :

A 4-digit password-based access control system built using an ATmega328P (Arduino). The system verifies user input and actuates a servo motor to simulate gate unlocking upon successful authentication.



Features:

4-digit password authentication

Dynamic password setting mode

Multiplexed 4-digit 7-segment display

Servo motor actuation using PWM

Buzzer feedback for success/failure

Debounced push-button input handling



Hardware Used:

Arduino (ATmega328P)

4-Digit 7-Segment LED Display

Push Buttons (Input / Enter / Reset)

Servo Motor

Buzzer

Resistors and external power supply


Working Principle
User enters a 4-digit password via push buttons.

Display updates using time-division multiplexing.

On confirmation:

Correct password → Servo rotates to unlock.

Incorrect password → Error indication and buzzer alert.

Reset button clears input and returns system to idle.



Pin Mapping (Core):

Segment Pins (A–G): D2–D8

Digit Select (D1–D4): D9–D12

Servo: A1

Buzzer: A3

Buttons: A2, A4, A5



Concepts Demonstrated:

Embedded C/C++ firmware design

GPIO-based display multiplexing

PWM-based actuator control

Event-driven input handling

Authentication logic implementation



Future Improvements:

EEPROM-based non-volatile password storage

Non-blocking timing using millis()

Custom PCB design

Relay-based real door lock integration
