#include <Servo.h>

Servo servo;

int pResistor = 0;

int value;

void setup(){
    pinMode (pResistor, INPUT);
    servo.attach(9);
    servo.write(0);
    Serial.begin(115200);
}

void loop(){
  value = analogRead(pResistor);
  Serial.print("Value: ");
  Serial.println(analogRead(pResistor));

  if (value > 300){
    servo.write(180);
  }
  else{
    servo.write(0);
  }
}
