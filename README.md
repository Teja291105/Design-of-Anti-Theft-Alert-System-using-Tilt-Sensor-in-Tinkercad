# NAME: TEJASHREE J
# REG NO: 212223060285
# Design-of-Anti-Theft-Alert-System-using-Tilt-Sensor-in-Tinkercad

**Aim:**

To measure the tilt Sensor using SW200D with Arduino UNO Board/ESP-32 using Tinker CAD. 

**Hardware / Software Tools required:** 
 
 - PC/ Laptop with Internet connection 
 - Tinker CAD tool (Online) 
 - Arduino UNO Board/ESP-32 
 - Tilt sensor(SW200D) 


**Circuit Diagram:**

<img width="1536" height="632" alt="Cool Sango-Amur" src="https://github.com/user-attachments/assets/3a9baeb4-44a6-4e1b-bf9f-0a6ab995733e" />


**Theory :**

The Arduino Uno is powered by the ATmega328P, an 8-bit microcontroller that runs at 16 MHz. It has 32 KB of flash memory, 2 KB of SRAM, and 1 KB of EEPROM. The board has 14 digital I/O pins (of which 6 can be used as PWM outputs) and 6 analog input pins. These pins allow the board to interface with various sensors, actuators, and other devices.The Arduino 67 Uno can be powered via a USB connection or an external power supply. The board has a built in voltage regulator to manage power from 7 to 12 volts. The board is programmable using the Arduino IDE (Integrated Development Environment), which supports a simplified version of C/C++. The code, known as a "sketch," is uploaded to the board via a USB connection. The Uno has a USB-B port, which is used for communication with a computer. The USB connection also powers the board when connected. The board includes a reset button that restarts the microcontroller, useful during programming and troubleshooting. The In-Circuit Serial Programming (ICSP) header allows for low-level programming of the microcontroller or firmware updates. The Uno has a built-in LED on pin 13, commonly used for simple tests and debugging.

**Procedur:**

1. Log in to Tinkercad, go to Circuits, and click Create New Circuit.

2. Add the Arduino Uno, PIR sensor, optional LED, 220-ohm resistor (if using LED), and jumper wires.

3. Connect PIR sensor VCC to 5V, GND to GND, and OUT to digital pin 2 on the Arduino.

4. If using an external LED, connect anode to pin 13 through a 220-ohm resistor and cathode to GND.

5. Open the Code editor, switch to Text mode, and write the Arduino program.

6. Start the simulation and test the PIR sensor by moving the virtual motion object near it.

7. If it doesn’t work, check wiring, fix any code errors, and adjust the sensor angle if needed.

8. Stop the simulation and save the circuit.


**Code:**

```
int ledPin=13; 
int inPin=7; 
void setup() 
{ 
 Serial.begin(9600); 
  pinMode(ledPin,OUTPUT); 
  pinMode(inPin,INPUT); 
} 
void loop() 
{ 
  int val=digitalRead(inPin); 
  if(val==0) 
  { 
    digitalWrite(ledPin,HIGH); 
  } 
  else 
  { 
    digitalWrite(ledPin,LOW); 
  } 
} 
```

**Output:**


<img width="673" height="398" alt="OP 5" src="https://github.com/user-attachments/assets/715f1563-c399-4ee5-be76-ddd28c057be8" />



**Result:**

 Thus measure the Tilt Sensor using SW200D with Arduino UNO Board/ESP-32 using Tinker CAD has been Verified Successfully.
