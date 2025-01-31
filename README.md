# Arduino-Modbus

Hardware: Arduino Uno, MAX485 module, RS485 Modbus RTU fuel sensor
Code to be uploaded to Arduino Uno. The fuel sensor transmits a level reading in Modbus RTU through RS485 which is converted to TTL by the MAX485 module, which is read by the Arduino Uno and displayed on the Arduino IDE Serial Monitor.

Connections between fuel sensor and MAX485 module
                          ________
Fuel Sensor RS485A -> A+ | MAX485 | DI -> 3
Fuel Sensor RS485B -> B- |        | DE -> 10
                   5V -> |        | RE -> 2
                  GND -> |________| RO -> 11
