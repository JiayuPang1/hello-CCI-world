# Original project file

## Link：
https://drive.google.com/drive/folders/18hnODSRry0hi66BkX_oMU7GAF2dtKhYo?usp=share_link


#include <Servo.h> 

Servo base; 

void setup() {
  // put your setup code here, to run once:
  base.attach(11); 

  Serial.begin(9600) ; 

}

void loop() {
  // put your main code here, to run repeatedly:
  if(!Serial.available()) return; 

  String str = Serial.readString();  

  if(str == "left") 
  { 
    base.write(175); 
  } 
  if(str == "right") 
  { 
    base.write(90); 
  } 
  if(str == "reset") 

  { 
    base.write(45); 
  } 
}
