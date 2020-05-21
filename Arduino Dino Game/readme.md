# Automatic Dino Game
## Main divisions
* Phototransistor
* Microcontroller
* Servo motor
* Code
## Troubleshooting
If the circuit does not work, then the issue is with one of the divisions above
check if all connections are proper and are connected to the power supply.

### Code
Check if this is right, as everything depends on this, if the code seems correct you can move on ahead.

### Servo 
  * Try this code 
  ```
  #include<servo.h>
  servo s
  void setup()
  {
  servo_test.attach(1); 
  }
  void loop()
  {
  s.write(90);
  delay(100);
  s.write(0);
  delay(100);
  }
  ```
  * If the servo oscillates ot should be fine, else you have to get a new servo.
  
  ### Phototransistor
  * Feed this code
  ```
  void setup()
  {
  serial.begin(9600);
  pinMode(2,INPUT);      // attach the phototransistor to pin A2 with similar setup of phototransistor on laptop screen.
  }
  void loop()
  {
  val=analogRead(2);
  val=map(val,0,255,0,100);
  serial.print(val);
  serial.print("\n");
  }
  ```
  * If there is a fluxuation of values in the serial monitor while the game is running, then the phototransistor is working, else you have to buy a new one.
  
### Arduino
  *If servo and phototransistor work but you cannot upload code to Arduino and if the IC is hot , you would have probably burnt it , but shorting an Arduino isn't easy , they have inbuilt mechanisms to prevent it so see if there are other issues as mentioned above before assuming that you have burnt your Arduino.

## If the space is being pressed at the wrong time
You have to adjust the phototransistor on screen to make it work properly by trial and error, also you may change the delay time as suited.

## Components
Just google the components or you can buy them in any electronic shop. They are easily available in many places. 
