---
date: 2026-07-25
categories:
  - Arduino IDE
  - ESP32
---

# Decrementing Blinky

This is my first project in embedded development.
<!-- more -->
- Used Arduino IDE and the required libraries for developing on esp32
- Opened up the classic blinky example
- Changed the default on/off loop to a for loop where I increase the delay and length of LED on (just to change it up a bit):

```CPP
for (int i = 0; i <= 10; i++) {
    digitalWrite(LED, HIGH);
    delay(i * 50 + 5 * i);
    digitalWrite(LED, LOW);
    delay(i * 50 + 5 * i);
 }
```

---
### Demo
<video controls width="100%">
  <source src="/media/Dec_blink.mp4" type="video/mp4">
</video>

---
### Full Code (Arduino)

```CPP
#define LED 2
void setup() {
  pinMode(LED, OUTPUT);
}

void loop() {
  for (int i = 0; i <= 10; i++) {
	digitalWrite(LED, HIGH);
    delay(i * 50 + 5 * i);
    digitalWrite(LED, LOW);
    delay(i * 50 + 5 * i);
  }
}
```

---

### Resources 
- [https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/)