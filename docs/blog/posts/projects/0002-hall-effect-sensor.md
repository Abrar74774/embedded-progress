---
date: 2026-07-31
categories:
  - Arduino IDE
  - ESP32
---

# Hall Effect Sensor

I learned that the esp32 comes with a built in hall effect sensor (at least some of the older models do), so I decided to test that out. Looked online for resources on this, and decided to follow the one from randomnerdtutorials <!-- more -->(link below). 

The code uses the `hallRead()` function, which is deprecated in the esp32 3.x library for arduino IDE, so I had to downgrade to 2.x.

### Demo
<video controls width="100%">
  <source src="/media/hall.mp4" type="video/mp4">
</video>



### Resources
1. [https://randomnerdtutorials.com/esp32-hall-effect-sensor/](https://randomnerdtutorials.com/esp32-hall-effect-sensor/)
