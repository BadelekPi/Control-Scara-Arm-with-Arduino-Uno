#include <Servo.h>

Servo myservo;  // tworzy objekt servo do kontroli naszego serwa
                // na większości płytek można stworzyć takich obiektów 12

int pos = 0;    // zmienna do zapamiętania pozycji serwa

void setup()
{ 
  myservo.attach(9);  // zdefiniowanie do którego portu podłączone jest serwo
} 

void loop()
{ 
  for(pos = 0; pos <= 180; pos += 1) // obrót od 0 do 180 stopni 
  {                                  // w krokach co 1 stopień
    myservo.write(pos);              // przekazanie do serwa obrotu o tyle ile jest zapisane w zmiennej 'pos'
    delay(15);                       // poczekaj 15ms, aby serwo osiągnęło ustaloną pozycje
  } 
  for(pos = 180; pos>=0; pos-=1)     // obrót od 180 do 0 stopni 
  {                                
    myservo.write(pos);              // przekazanie do serwa obrotu o tyle ile jest zapisane w zmiennej 'pos'
    delay(15);                       // poczekaj 15ms, aby serwo osiągnęło ustaloną pozycje
  } 
}
