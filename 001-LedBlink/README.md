# Led Blink
#### Lampeggio del led presente nella scheda

Il led presente nella scheda è collato al pin 2 (DevKit V1, nella V4 il led non è presente)
```
#define LED_PIN 2 //ON Board LED GPIO 2
```

Configuriamo il pin come output
```
void setup() {
  // Set pin mode
  pinMode(LED_PIN, OUTPUT);
}
```

Accendiamo e spegnamo il led ad intervalli di 500ms 
```
void loop() {
  delay(500);
  digitalWrite(LED_PIN, HIGH);
  delay(500);
  digitalWrite(LED_PIN, LOW);
}
```

<p align="center">
  <img src="https://github.com/filippo-bilardo/ESP32-DEVKIT/blob/main/001-LedBlink/LedBlink.png?raw=true" alt="Led blink example"/>
</p>

