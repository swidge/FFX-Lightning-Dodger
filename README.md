# FFX Lightning Dodger

This simple Arduino project automates the lightning dodging required to obtain the Venus Sigil for Lulu's Celestial Weapon. It uses a photoresistor to detect the screen flash and uses a servo motor to press a controller button. The performed dodges are counted and displayed on an LCD.

## Required Parts

-   Arduino Uno or Arduino compatible board
-   Photoresistor
-   ~5k-10k ohm resistor
-   SG90 servo motor with an arm
-   LCD1602 module
-   10k ohm potentiometer
-   Breadboard
-   Jumper wires

## Wiring Example

Note: This example was autogenereated by circuit.io. FFX Lightning Dodger is using different pins on the Arduino. If you want to use the exact pins in this wiring diagram, you will need to change the pin definitions in the code.
![Wiring diagram](https://i.imgur.com/yaJA2ae.png)

## Example Setup

I have attached the photoresistor to a small breadboard that I taped to a jug in order to mount it against the TV. The closer you can get the photoresistor to the TV, the easier it will be to calibrate the threshold and avoid false positives.

-   Adjust the `threshold` variable until it is only triggering the servo when the screen flashes. For my TV, photoresistor, and placement, the value was about 350.
-   You may need to adjust the `startDegs` variable to set the starting position of the servo or attach the arm such that its in the correct position.

![FFX Lightning Dodger](https://i.imgur.com/V69QE2F.jpg)
![PS4 Controller with servo attached](https://i.imgur.com/zpi1vIx.jpg)
