# Firmware of my clock pcb contains info how it will be programmed
Software needed- Arduino IDE \
Microcontroller used- ESP32 (So ESP32 board will be installed in board manager otherwise ESP can't be programmed) \
Libraries to be installed- TM1637 Library by Avishay Orpaz

# What do you define in your code?
1. Include the library used-> **#include <TM1637Display.h>**
2. Define CLK & DIO pins numbers-> **#define CLK 8 and #define DIO 9**
3. List the variable names & the logic you will be running.
4. In void setup-> write the one time actions like pin modes, library initializations & serial monitor configurations.

# What does the animation.ino do?
It is my display testing code. \
In it I broke down Upper & Lower Segments in parts. \
In output result the display's upper and lower segments glows

