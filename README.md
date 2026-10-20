# Digital Clock Display
It is a printed circuit board clock module. 
My project is inspired from easily available LED Display Module. I plan to make PCB around its circuitry and logics.
The LEDs on this display module works because of an IC called TM1637 IC.
The TM1637 IC can run LED displays & Keyboards in 6by8 and 2by8 matrix repectively.


<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/ee46d2f1-e65e-416a-8f27-b4b746badebf" />


# Core features and specifications of TM1637 IC:
​At the heart of the design is the TM1637 IC, a specialized LED driver and keyboard scan interface.

1. ​**LED Display Driving**: Capable of managing an 8-segment by 6-grid matrix configuration for bright, multiplexed numeric or alphanumeric displays.

2. ​**Keyboard Scanning**: Supports an integrated 2 by 8 key matrix scanner, allowing for compact user input alongside the display without requiring extra microcontroller pins.

3. ​**Minimal Pin Count**: Communicates via a simple two-wire serial interface (CLK and DIO), saving valuable GPIO pins on your microcontroller (such as an Arduino, ESP32, or STM32).

4. **​Custom Form Factor**: Designed from scratch to fit a specific layout and form factor optimized for clean integration into custom enclosures or electronics projects.

<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/4b86bff5-dba3-41b1-91d1-78d7a9799000" />


# Capibilities and Display modes:
1. **Numbers & Selected Alphabets**: Render numeric data and custom alphanumeric characters.
2. **​Temperature Monitoring**: Display real-time temperature readings in both Celsius °C and Fahrenheit °F.
3. ​**Scrolling Text**: Smoothly scroll messages or status updates across the 4 digits.
4. ​**Counter & Timer**: Function as a digital stopwatch, countdown timer, or event counter.
5. ​**Smart Alarm Clock**: Expandable with an external RTC (Real-Time Clock) time module to build a full-featured desk clock and alarm.


# Hardware specifications- 
The custom PCB layout keeps external component counts minimal while maximizing functionality:
1. **Driver IC**: 1 × TM1637 IC
2. **Display Elements**: 30 total LEDs soldered directly to the board (28 LEDs forming the 4-digit 7-segment display + 2 LEDs forming the central colon).
3. **​Passive Components**: 2 resistors and 2 capacitors.
4. **External Requirements**: ESP32 microcontroller and jumper cables for connection.
5. **​Circuit Configuration**: Designed to support either common anode or common cathode LED configurations depending on layout needs.


# TM1637 IC pin mapping & architecture 
The TM1637 IC handles multiplexing efficiently using a minimal pin layout: \
​1. **Grid Pins (4 of 6 Used)**: The IC features 6 grid pins total. Because this is a 4-digit display, exactly 4 grid pins are utilized to sequence each digit. \
2. **​Segment Pins (All 8 Used)**: The IC features 8 segment pins. 7 pins are dedicated to driving the individual segments of the 7-segment display, while the 8th pin drives the central colon LEDs. \
3. **​Communication Interface**: Connects to the ESP32 via a simple two-wire serial interface (CLK and DIO), preserving valuable GPIO pins.

<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/cc25d200-0f94-4601-b434-81924b6c133b" />






