# bocce_measurer
bocce ball measuring device using echo ping sensor and an arduino

This project is built using the following parts - 

- Arduino Uno (or Sparkfun Redboard)
- HC-SR04 echo ping sensor
- 5 mW laser module from Sparkfun (COM-09906)
- PN2907A PNP transistor
- Graphic LCD (84x48, Nokia 5110 from Sparkfun, LCD-10168)
- Switch and 4 AA batteries


- The button is connected to pins 2 and GND, no power
- The echo and trigger pins from the HC-SR04 are connected to pins 7 and 8, powered by 5V
- The LCD is connected to pins 4, 5, 6, 11, and 13, powered by 3.3V
- The transistor is connected to pins 9, and 5V, and the laser

The Arduino code initially turns on the laser for aiming, and waits for the button signal. 
When signaled, the laser will blink, and the screen will display Measuring, followed by the distance measured in cm.
The loop then repeats and waits for another button push, while displaying Idle on the screen.