---
date: 2026-08-19
categories:
  - ESP-IDF
  - ESP32
---
# Blinky Example using ESP-IDF

Time to get into using the vendor SDK, which for my ESP32 would be the ESP-IDF (Integrated Development Framework). I've read about how the Arduino IDE is not much used for production used, so I plan to learn this framework, and hopefully embedded dev without using framework as well in the future.
<!-- more -->
For this project, much of my time was spent on getting to install the SDK itself. Initially I used the online installation manager to download and install ESP-IDF v6. However, it seems the installation was a bit weird. I couldn't find the uninstall on Control Panel, which probably means it wasn't installed as a Windows application, but rather a bunch of libraries. I had problems using it with vscodium. So later on I downloaded the v5.5, after which I could successfully use the SDK with vscodium. 

I opened up the `blink` example that they provided. Flashed it to the esp32, but I wasn't seeing the LED blink. Apparently I missed setting the GPIO to 2 using menuconfig, so I did that and got it to work.

I later on changed the code a little bit to make the blinking decrement from fast to slower like I did in [my first project](./0001-decrementing-blinky.md)