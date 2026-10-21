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
The TM1637 IC can run LED displays & Keyboards by making matrix connections.

# What can we display on it?
1. Alphanumerics
2. Temperature in degree celsius or fahrenheit
3. Scrolling text
4. Number counter or timer
5. Alarm clock display

# Schematic Diagram
<img width="1340" height="525" alt="Screenshot 2025-10-16 113158" src="https://github.com/user-attachments/assets/8d00fe10-69a6-444a-a991-aa0b4b018c8b" />
Layout of the PCB was based on this schematic diagram which contains TM1637 IC, LEDs, etc. 

# TM1637 IC connections
<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/cc25d200-0f94-4601-b434-81924b6c133b" />

1. 8 SEGMENT pins & 4 GRID pins on the IC will be used to make LED display.
2. GRID pins will be used for each digit in a display. IC has 6 grid pins. I am making a 4 digit 7 segment display. So, I will only use 4 grid pins.
3. SEGMENT pins will be used for each segment in a display. IC has 8 segment pins. I am making a 4 digit 7 segment display. So, I will use all pins because 7 pins for 7 segments & 1 for colon leds.


# BOM

| Part | What it's for | Qty | Unit | Total | 
| --- | --- | --- | --- | --- | 
| [TM1637 IC](https://www.sunrom.com/p/tm1637-soic20-led-display-and-keypad-driver-ic) | on board led controller on the pcb board | 1 | $0.31 | $0.31 |
| [Leds](https://www.sunrom.com/p/red-led-3mm) | To make led segments on the pcb board | 30 | $0.04 | $1.20 | 
| [Resistor](https://www.sunrom.com/p/0r5-1-1206-smd-shunt-resistor-05-ohms-0125w-18w) | to protect the on board ic when powered on | 2 | $0.04 | $0.08 | 
| [Capacitor](https://www.sunrom.com/p/10uf-106-smd-50v-x7r-1206) | to protect the onboard ic from power surges | 2 | $0.03 | $0.06 | 
| [ESP32-C3 Development Board](https://robu.in/product/esp32-c3-development-board-with-soldering/) | microcontroller board | 1 | $3.00 | $3.00 | 
| [Jumper wires](https://robu.in/product/male-to-female-jumper-wires-40-pin-40cm/) | to connect pcb pins to esp32 pins | 1 | $1.02 | $1.02 | 
| [Printed Circuit Board](https://robu.in/product/online-pcb-manufacturing-service/) | making the project | 1 | $12.20 | $12.20 | 
| **Parts subtotal** | — | — | — | **$17.87** | 
| **Tax & shipping** | — | — | — | **$9.00** | 
| **Total** | — | — | — | **$26.87** | 










