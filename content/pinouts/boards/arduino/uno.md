# Arduino Uno

## Board Specifications

<table>
  <tr>
    <td>Microcontroller</td>
    <td>ATmega328P</td>
  </tr>
  <tr>
    <td>IO Voltage</td>
    <td>5V</td>
  </tr>
  <tr>
    <td>Input Voltage / VIN</td>
    <td>7-12V</td>
  </tr>
  <tr>
    <td>Digital IO Pins</td>
    <td>14</td>
  </tr>
  <tr>
    <td>PWM IO Pins</td>
    <td>6</td>
  </tr>
  <tr>
    <td>Analog IO Pins</td>
    <td>6</td>
  </tr>
  <tr>
    <td>Max Current per Pin</td>
    <td>20mA</td>
  </tr>
  <tr>
    <td>Clock Speed</td>
    <td>16MHz</td>
  </tr>
  <tr>
    <td>Length</td>
    <td>68.6mm</td>
  </tr>
  <tr>
    <td>Width</td>
    <td>53.4mm</td>
  </tr>
  <tr>
    <td>Height</td>
    <td>13mm</td>
  </tr>
  <tr>
    <td>Weight</td>
    <td>25g</td>
  </tr>
</table>

## Pinout

<img src="/uno-pinout.svg"></img>

### D0 - D13

The Uno board has a total of 14 Digital IO pins.
Pins 3, 5, 6, 9, 10 and 11 have Hardware PWM Capability.
Each pin can only output up to 40mA max. (Only recommended up to 20mA).
The total current provided by all pins together can only reach up to 200mA!

### A0 / A1 / A2 / A3 / A4 / A5

The Uno board has a total of 6 Analog Input pins provided by a internal ADC (Analog to Digital Converter)
These pins mainly serve as Analog inputs, but can be used as standard Digital IO Pins.

### SDA / SCL

These pins are dedicated to I2C Communication.

### AREF

Analog Reference. Provides a voltage reference for Analog Inputs.

### IOREF

Input / Output Reference. Provides a voltage reference with which the microcontroller operates.

### RESET

Bringing this pin to a logical LOW will cause the microcontroller to reset. 

### +3V3

This pin provides regulated 3.3V to power components.

### +5V

This pin provides regulated 5V to power components.
(It is possible- but not recommended- to feed 5V in via this pin.)

### VIN

The UNO board can be powered by 5-20 volts, however Arduino recommends to only use between 7-12 volts. Over this range can make the regulator overheat, and below this range may simply not be enough for the board to run.