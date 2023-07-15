# Esp32-Puerto-Serial-No-Funciona en setup

### Este proceso no muestra la depuracion del puerto serial
```c++
void setup()
{
  Serial.begin(115200);
  Serial.println("Hola Mundo");
}

void loop()
{
}
```

### Para ver el puerto serial agregar un retardo
```c++
void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  //Retardo de cinco segundos
  delay(5000);

  //Imprime el mensaje de depuracion
  Serial.println("Hola Mundo");
}

void loop()
{
}
```

Esto pasa simplemente porque el esp32 escribe muy rapido en el puerto serial al momento de abrir el puerto serial no se visualiza nada pero al agregar el retardo de cinco segundos da tiempo suficiente para abrir el puerto serial
