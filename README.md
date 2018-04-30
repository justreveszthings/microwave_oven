# microwave_oven
Control program for microwave oven with PIC16F18857 (X2C+ Development Board).

Timer: The backing time can be set up with potentiometer in 20-second intervals. The maximum value of timer is 2 minute. To display the preset time use UART communication.

Buttons: Cooking can be start and stop with S1 button (START/STOP button). The S2 button simulates the state of the door. If the button is pressed the microwave oven door is open. If the button is released the microwave oven door is close.

Status LEDs: The LED1 symbolizes state of magnetron. If the LED is turned on the baking is in progress. If the LED is turned of then the magnetron is not active. The LED2 represents the internal lighting. If the LED is turned on the oven interior light is active.

Baking process: The cooking process can be start with pressing the START button. The cooking process starts if the door is closed and the START button is pressed. During the cooking process the time indicator LED3 is blinking with 100 ms period and the magnetron is turned on. Indicate the remaining time on the serial port.

The cooking process can be paused with opening of the door. If the door is opened the cooking process have to be stopped immediately, but the LED3 is blinking continuously indicating that the cooking program is in progress. To continue the cooking process the user have to close the door and have to press the START button.

Pressing the STOP button stops the cooking process. In the case when the cooking time has elapsed the cooking process is halted also.

Lighting: The oven interior light is turned on during cooking process or the door is open.
