# Controle-de-Microservo-com-Potenci-metro-no-Arduino-IoT

<img width="1297" height="675" alt="image" src="https://github.com/user-attachments/assets/739bfba1-65d2-41af-81f7-17c63200c101" />
 Resumo da aula

Nesta aula, aprendemos a controlar um **microservo usando um potenciômetro**. Utilizamos o Arduino e o Tinkercad para montar e simular o circuito, praticando a leitura de valores e o controle do servo por programação.




// C++ code //
#include <Servo.h>

Servo servoMotor;

int potenciometro = A0; 

int valorLido; 
int angulo; 

void setup() {

    servoMotor.attach(9); 

}

void loop() {

    valorLido = analogRead(potenciometro); 
    angulo = map(valorLido, 0, 1023, 0, 180); 
    servoMotor.write(angulo);

    delay(15); 
}







https://www.tinkercad.com/things/71NdkxF3oN1-stunning-snicket-albar/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard&amp;sharecode=XVlKypIMPOg2GWlY5iObM1Q5xHZUpAMXkv2xXxz3410
