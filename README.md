# PWM Signals Project
Arduino-Based LED Control Using PWM Signals: Developed an Arduino-based LED project that utilizes Pulse Width Modulation (PWM) signals to control LED behavior.

# Hardware Component
- Arduino UNO - Microcontroller that generates PWM signals to control the timing, brightness, and behavior of the LEDs.
- Breadboard - A platform used to connect and organize the components of a circuit.
- Jumper cables(x5) - Used to establish electrical connections between the Arduino, breadboard, resistors, and LEDs.
- Resistors(330Ω) - Components that limit the electrical current flowing through the LEDs to prevent damage.
- LED - Light-emitting components that produce light, with their brightness controlled by the PWM signals from Arduino.

# Wiring 
- GND Pin → (-) terminal of the breadboard
- Pin 11 (~) → 21h → 330Ω Resister (21j → 7h) → jumper cable (6h → (-) terminal) → Red LED (6j → 7j)  
- Pin 6 (~) → 27b → 330Ω Resister (27c → 17c) → jumper cable (16b → (-) terminal) → Yellow LED (16d → 17d)

# Code
**1. LED Variables:** The integer number assigned to each LED variables represents the Arduino pin #, with only ~ pins supporting PWM.

**2. Initial Values:** brightness starts at 0 and fadeAmount is set to 5, causing the LED to initially brighten by 5 each loop.

**3. Set pins as outputs:** pinMode() function sets the LED pins as outputs so the Arduino can control them. 

**4. PWM Signal:** analogWrite() function sends PWM signal to control the LED's brightness from 0 to 255.

**5. Change Brightness:** brightness = brightness + fadeAmount which changes the LED's brightness by 5 each loop, either increasing or decreasing depending on value of fadeAmount.

**6. Reverse Fading:** The if statement checks whether brightness reaches 0 or 255 and reverses fadeAmount.

**7. Delay:** If 0 < brightness < 255, the code waits 30 milliseconds before continuing the next line of code.
  

