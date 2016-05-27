# rpi-temposcope

JD-VCC -> 5v pin 2
nearest GND -> GND pin 6
IN1 -> GPIO17 pin 11
furthest VCC -> 3.3v pin 1

```
$ echo 17 > /sys/class/gpio/export
$ echo out | sudo tee /sys/class/gpio/gpio17/direction
$ echo 1 | sudo tee /sys/class/gpio/gpio17/value
```
