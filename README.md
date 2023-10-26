## Onshape Certification Prep: The Swing Arm



### Assignment DescriptionL: for this assignement we were supposed to create a swing arm using onshape, using some complicated steps.

 * Create this part in Onshape. 


### Evidence

  * ![image](https://github.com/Mulamba53/engineering3/assets/143534921/3c5cf3cf-57e5-4b33-9885-96c37b7d0371)
  * ![image](https://github.com/Mulamba53/engineering3/assets/143534921/ac35dbff-f4e5-4cd4-9e83-2055dc6d4f74)



### Part Link 

  * https://cvilleschools.onshape.com/documents/d10cb16dbbec7c77c4a9579f/w/c7b88cf4387e01565ace8d16/e/e63d5010121b85b8d8393555?renderMode=0&uiState=65314de9d569811e5d8be672

### Reflection:This onshape assignement was both fun and challenging at the same time, we had to design a swing arm using onshape, I was able to finish this with the help of the teacher and a couple of my peers

  * 

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 ## Practice Design from Drawings: The Hanger



### Assignment Description: This was the first Onshape assignment we got this quarter we were supposed to design a hanger using few different methods different from last year's onshape projects.


### Evidence:![image](https://github.com/Mulamba53/engineering3/assets/143534921/065b0c79-cec0-4d6c-8580-8593532ea353)

![image](https://github.com/Mulamba53/engineering3/assets/143534921/e3ceaa07-571c-4b92-832f-82f6ae0a9b75)



### Part Link :https://cvilleschools.onshape.com/documents/f68f33b91914a0754444bba7/w/57c5daffc7b46cb60a4c0ad0/e/3e953b225dd3f98c4596a155?renderMode=0&uiState=653abd9ee3472f3645e79b99


### Reflection: This assignment was a bit easier than the swing arm and it was fun doing it.

___________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

 ## CircuitPython Servo



### Description & Code 




Get a 180° micro servo to slowly sweep back and forth between 0 and 180°. Spicy part: Now control the servo with 2 buttons. The servo only moves if you are pushing a button.

import time import board from digitalio import DigitalInOut, Direction, Pull

btn1 = DigitalInOut(board.D9) btn1.direction = Direction.INPUT btn1.pull = Pull.DOWN

btn2 = DigitalInOut(board.D10) btn2.direction = Direction.INPUT btn2.pull = Pull.DOWN

while True: if btn1.value: print("BTN1 is pressed")

if  btn2.value:
    print("BTN2 is pressed")
   

time.sleep(0.1) # sleep for debounce


### Evidence

### Wiring

![276354963-5c4af0d8-5d09-405a-83b1-e99f6da88e4a](https://github.com/Mulamba53/engineering3/assets/143534921/e5199bf9-fcb1-4276-baa9-d9244aaa8caa)


### Reflection

I learn that how to do the code for this assingment. and I enjoy working on this assmingment I know it was hard but I work hard and never give up and I know I can do it.



______________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

## CircuitPython Distance Sensor


Description & Code Snippets
I've broken the assignment into 3 stages, to make your life easier:

Use the HC-SR04 to measure the distance to an object and print that out to your serial monitor or LCD in cm. Next, you will get the neopixel to turn red when your object is less than 5cm, and green when its 35cm. Ignore the blue and 20cm for now, let's just keep it simple. For your final version of this code, you'll smoothly shift the color of the onboard neopixel, corresponding to the distance, according to the graphic below. (Neopixel should stay red when below 5cm and green when above 35cm)

if  btn2.value:
    print("BTN2 is pressed")
   

time.sleep(0.1) # sleep for debounce

### Evidence
https://www.wevideo.com/class#view-media/3196343174/
https://www.wevideo.com/class#view-media/3196343047/
### Wiring 
![276663497-21dbde8e-a2a1-4571-a597-396530ac50ab](https://github.com/Mulamba53/engineering3/assets/143534921/acd57cc8-bf1e-4a5a-a203-7e3ad7ad3b11)

### Reflection

In this assingment the coding was very short and more wiring and the goal was that it should show us the Distance and help us to get use to coding.
__________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________


## Motor_control


### Description & Code 

The goal of the assignment was to control motor with the speeding button.
I accomplish to my goal by using goal and ask firend for help and using my idea also I take a step by step top accomplish to my goial.
motors can draw a lot more juice (current) than LEDs. In fact, they draw so much current, we don't want to power them directly from the Arduino. That might fry the Arduino. So, we will power our motor directly from a 6 V battery pack.

### Evidence
*  https://www.tinkercad.com/things/brGb4NP2EIS-writing-the-code/editel?lessonid=E2IR521ISCBY8RV&projectid=O73WOLIISCC2EWG#/lesson-viewer
* https://www.wevideo.com/class#view-media/3196420050/
* import time
import board
import pwmio
from analogio import AnalogIn
from digitalio import DigitalInOut, Direction, Pull

motor = pwmio.PWMOut(board.D9, frequency=50)




pot = AnalogIn(board.A1)



while True:
  print(pot.value)
  time.sleep(0.1)
  motor.duty_cycle=pot.value

### Wiring

### ![273625642-f6ea0824-a370-4ba4-8cf4-1b1a726c3167](https://github.com/Mulamba53/engineering3/assets/143534921/30011917-a453-4931-a94b-37692f7d48b1)


### Reflection
This assignment was fun to do, because you could control how fast the motor goes by tuning potentiometer. 
