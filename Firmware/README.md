# Firmware of my clock pcb contains info how it will be programmed
Software needed- Arduino IDE \
Microcontroller used- ESP32 (So ESP32 board will be installed in board manager otherwise ESP can't be programmed) \
Libraries to be installed- TM1637 Library by Avishay Orpaz

# What do you define in your code?
1. Include the library used-> **#include <TM1637Display.h>**
2. Define CLK & DIO pins numbers-> **#define CLK 8 and #define DIO 9**
3. List the variable names & the logic you will be running.
4. In void setup-> write the one time actions like pin modes, library initializations & serial monitor configurations.
5. In void loop-> white the task that will happen one after another after some delay.

# How does the animation.ino work?
It is my display testing code. \
In it I broke down Upper & Lower Segments in parts. \
In output result the display's upper and lower segments glows in some manner. \
[Refer video **DisplayAnimation.mp4**]

# Feature of the Display?
Refer to the video [**FeaturesOfDisplay.mp4**] to have an idea of my display working. \
I didn't add code used in this video because it needs seperate explaination of circuit diagram & its firmware's working.

__THANK YOU__
