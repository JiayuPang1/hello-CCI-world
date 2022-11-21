# Machine Manifesto: A public interactive artwork combining VR and interactive devices
____________
## The Fianl Project

## · Introduction

#### The “Machine Manifesto” is an immersive public art concept work that combines VR games and interactive installations. Through the immersive experience of players in the VR game world and the physical operation of external mechanical devices, it not only promotes the communication of the project concept but also breaks the limitation of the number of people who experience VR public devices, and enhances the participation of ordinary audiences. The research paper describes the iterative design process of "Mechanical Manifesto", the specific introduction of the project concept and related technologies, the evaluation of the emotional experience of the entire immersive art concept work after the final project test, and the outlook for the future optimization direction of the project. In addition, the project aims to make players also part of the visual expression of VR public installations by testing the combination of VR games and physical installations. While promoting concept communication, further explore whether the combination of VR and interactive devices can enable players and ordinary audiences to gain more interactive experience and a sense of participation.

## The Vedio of the Final Project：
https://youtu.be/kuVG5XKM5Uk

## · Original Project File Link：
https://drive.google.com/drive/folders/18hnODSRry0hi66BkX_oMU7GAF2dtKhYo?usp=share_link

## The code of the Arduino：

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


## Progress Weekly

### WEEK 01 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2001%20Process.md

### WEEK 02 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2002%20Process.md

### WEEK 03 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2003%20Process.md

### WEEK 04 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2004%20Process.md

### WEEK O5 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2005%20Process.md

### WEEK 06 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2006%20Process.md

### WEEK 07 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2007%20Process.md

### WEEK 08 Link：
https://github.com/JiayuPang1/hello-CCI-world/blob/main/Final%20Project/Week%2008%20Process.md
