# Esp32-Puerto-Serial-No-Funciona en setup

### Este codigo no se muestra al abrir el puerto serial
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
