# ESP8266
This sketch contains minor changes to the Arduino sketch
that allows one to use an ESP8266 ( Wemos D1 mini in my case) as 
an ISP.

Compile using Arduino IDE

- Board: esp8266 > LOLIN(WEMOS) D1 mini (clone)

Programmer pinout

- D8: RST
- D7: MOSI
- D6: MISO
- D5: SCK

Avrdude command

```
$ avrdude -c avrisp -patmega328p -P /dev/ttyUSB0 -b 19200
```

To upload a sketch to the ATtiny85.
After installing the ISP sketch,
change the board type to ATtiny85.

Note this assumes you have already installed Arduino IDE support for the ATtiny85


