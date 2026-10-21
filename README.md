# DIGITAL CLOCK DISPLAY
<p float="center">
  <img src="https://github.com/user-attachments/assets/e96ec315-8ea1-40f4-b74b-474f04fde427"  width="39%" />
  <img src="https://github.com/user-attachments/assets/f787647e-1b9d-46dc-9fc7-244b52571333" width="39%" />
</p>

This is a Clock PCB Display that can display numbers using LEDs on it. It uses ESP32 and Arduino IDE Firmware. \
I designed this by referencing the 7 Segment Clock Module I bought. I studied its datasheet, connection diagrams, IC working and logics to implement it in my PCB. 

<p float="center">
  <img src="https://github.com/user-attachments/assets/ee46d2f1-e65e-416a-8f27-b4b746badebf" width="30%" />
  <img src="https://github.com/user-attachments/assets/4b86bff5-dba3-41b1-91d1-78d7a9799000" width="65%" />
</p>

The LEDs on this display module works because of an IC called TM1637 IC.
The TM1637 IC can run LED displays & Keyboards by making LED matrix.

# What can we display on it?
1. Alphanumerics
2. Temperature in degree celsius or fahrenheit
3. Scrolling text
4. Number counter or timer
5. Alarm clock display

# BOM used

| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Row 1, Col 1 | Row 1, Col 2 | Row 1, Col 3 |
| Row 2, Col 1 | Row 2, Col 2 | Row 2, Col 3 |



# My project specifications- 
4 Digits made with 7 segments with one colon between them. \
Total 30 leds, 2 resitors, 2 capacitors and 1 TM1637 IC required that will be soldered on the PCB. \
Other components needed for running the PCB are jumper cables and ESP32 microcontroller. \
There are two types of led connection we can make- common anode or common cathode configuration.

# TM1637 IC connections
1. 8 SEGMENT pins & 4 GRID pins on the IC will be used to make LED display.
2. GRID pins will be used for each digit in a display. IC has 6 grid pins. I am making a 4 digit 7 segment display. So, I will only use 4 grid pins.
3. SEGMENT pins will be used for each segment in a display. IC has 8 segment pins. I am making a 4 digit 7 segment display. So, I will use all pins because 7 pins for 7 segments & 1 for colon leds.


<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/cc25d200-0f94-4601-b434-81924b6c133b" />






