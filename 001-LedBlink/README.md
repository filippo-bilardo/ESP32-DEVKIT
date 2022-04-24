# Led Blink
#### Lampeggio del led presente nella scheda

Il led presente nella scheda è collato al pin 2 (DevKit V1, nella V4 il led non è presente)
```C
#define LED_PIN 2 //ON Board LED GPIO 2
```

Configuriamo il pin come output
```C
void setup() {
  // Set pin mode
  pinMode(LED_PIN, OUTPUT);
}
```

[Sez](#lampeggio-del-led-presente-nella-scheda)
Accendiamo e spegnamo il led ad intervalli di 500ms 
```C
void loop() {
  delay(500);
  digitalWrite(LED_PIN, HIGH);
  delay(500);
  digitalWrite(LED_PIN, LOW);
}
```
<details><summary>CLICK ME</summary>
#### We can hide anything, even code!

    ```ruby
      puts "Hello World"
    ```
</details>

<p align="center">
  <img src="LedBlink.png?raw=true" alt="Led blink example"/>
</p>

