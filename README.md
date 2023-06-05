# Esp32-Puerto-Serial-No-Funciona en setup

### Este codigo no se muestra la impresion del puerto serial en setup
```c++
void setup() 
{
Serial.begin(115200);
Serial.println("Hola Mundo");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

### PARA VER EL PUERTO SERIAL AGREGAR UN RETARDO
```c++
void setup() 
{
Serial.begin(115200);
delay(5000);
Serial.println("Hola Mundo");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

Esto pasa simplemente porque el esp32 escribe muy rapido en el puerto serial al momento de abrir el puerto serial no se visualiza nada pero al agregar el retardo de cinco segundos da tiempo suficiente para abrir el puerto serial
