# Electronic-circuit

## How to work with Arduino and build a circuit in tenikercad like this:  
<img src="https://github.com/HAN6661/Electronic-circuit/assets/173714836/f322b0a5-c1f7-4848-932b-6fe89a52af18.jpg" width="50%" height="50%">

### Tools 
Components Needed:

1- 1 x Arduino Uno

2- 6 x Servo Motors

3- External power supply

4- Breadboard and connecting wires

### First you gone download the Arduino 1.8.19

### Open the arduino 
<img src="https://github.com/HAN6661/Electronic-circuit/assets/173714836/d5ba6365-5199-49b3-b59a-aee7cf4f0374.jpg" width="50%" height="50%">


### Open sweap and read the example 
<img src="https://github.com/HAN6661/Electronic-circuit/assets/173714836/e3d83eaa-c640-4bd2-bd98-44b1ba253738.jpg" width="50%" height="50%">

### Then make the code to start the 6 servo 
```

#include <Servo.h>

Servo myservo1;  // create servo object to control a se
Servo myservo2;      // twelve servo objects can be created on most boards
Servo myservo3;
Servo myservo4;
Servo myservo5;
Servo myservo6;

int pos = 0;    // variable to store the servo position

void setup() {
  myservo1.attach(11);
  myservo2.attach(10);
  myservo3.attach(9);
  myservo4.attach(5);
  myservo5.attach(3);
  myservo6.attach(4);// attaches the servo on pin 9 to the servo object
}

void loop() {
  for (pos = 0; pos <= 180; pos += 1) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    myservo1.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15 ms for the servo to reach the position
  }
  for (pos = 180; pos >= 0; pos -= 1) { // goes from 180 degrees to 0 degrees
    myservo1.write(pos);              
    delay(15);                       
  }
  for (pos = 0; pos <= 180; pos += 1) { 
    // in steps of 1 degree
    myservo2.write(pos);           
    delay(15);                       
  }
  for (pos = 180; pos >= 0; pos -= 1) { 
    myservo2.write(pos);             
    delay(15);                      
  }
  for (pos = 0; pos <= 180; pos += 1) { 
    // in steps of 1 degree
    myservo3.write(pos);           
    delay(15);                       
  }
  for (pos = 180; pos >= 0; pos -= 1) { 
    myservo3.write(pos);             
    delay(15);                      
  }
  for (pos = 0; pos <= 180; pos += 1) { 
    // in steps of 1 degree
    myservo4.write(pos);           
    delay(15);                       
  }
  for (pos = 180; pos >= 0; pos -= 1) { 
    myservo4.write(pos);             
    delay(15);                      
  }
  for (pos = 0; pos <= 180; pos += 1) { 
    // in steps of 1 degree
    myservo5.write(pos);           
    delay(15);                       
  }
  for (pos = 180; pos >= 0; pos -= 1) { 
    myservo5.write(pos);             
    delay(15);                      
  }
  for (pos = 0; pos <= 180; pos += 1) { 
    // in steps of 1 degree
    myservo6.write(pos);           
    delay(15);                       
  }
  for (pos = 180; pos >= 0; pos -= 1) { 
    myservo6.write(pos);             
    delay(15);                      
  }
}
```


### Here we use 6 servo with power supply 
