# UART Bridge Design Explanation
Notes regarding UART Brdige design choices and specs.

## ESP32-PICO-MINI-02
- Espressif's tiny ESP32 module for bluetooth and other minor applications
- it's literally made to trasmit UART serial over bluetooth for a computer to pick up over a terminal emulator

- Sparkfun
  - plenty of documentation for below products:
  - Bluetooth Bridge module using here: https://www.sparkfun.com/sparkfun-bluesmirf-v2-headers.html
  - dev board for if we need to do anything other than bluetooth bridge-ing: https://www.sparkfun.com/sparkfun-esp32-qwiic-pro-mini.html
  - USB to serial breakout board to program the ESP32 over serial rx/tx: https://www.sparkfun.com/sparkfun-serial-basic-breakout-ch340c-and-usb-c.html
  - video for ESP32 minimal setup: https://youtu.be/tQ0dL_9M1wI?si=PeC6zGlJdLPajcbK 

## Archived Ideas
- building a custom Bluetooth module w/ an SoC
  - would be a cool project, but time consuming due to special antenna traces, SoC programming, extra tools, etc
  - we can just integrate Espressif's module into a small PCB and attach it to the micromouse motherboard's USART jumper pins