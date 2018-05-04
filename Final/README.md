# Project Writeup

## CD (for Color Disc)

### Project Goals

To make a "music player" that turns colorful patterns made by visitors into music. 

More specifically, the visitors can put colorful paper scraps on a disc, make it spin (and stop spinning,) and the system will translate the disc into music.



### Technical decisions

To achieve the goal, I use transparent cast acrylic and paper scraps in bright colors as the "disc". I also put an array of four LDRs (light dependent resistors) underneath and RGB sensor above the disc to "read" it. As the visitor pushes a button, a DC motor starts to rotate, driving the plate to spin. Meanwhile, the LDRs and RBG sensor send brightness and RGB data of a certain radius of the disc to an Arduino UNO. The Arduino program then maps the realtime data (weighted brightness level and color of one point) to different music files, which will finally be played by a Adafruit Music Maker Board.



### Schematic

(breadboard version)

![colordisc_schematic_0429](images/colordisc_schematic_0429.jpg)



### Parts list

Sensors

- RGB Color Sensor (TCS34725)
- Mini Photocells (LDRs)

Microprocessors

- Arduino UNO
- Adafruit Music Maker Shield

Other major components

- DC Motor
- Speaker



### Photos

#### Overall

the operational project (04/26)

![operational_1](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/operational_1.jpg)

![operational_2](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/operational_2.jpg)

![using](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/using.png)



#### Components

Motor & push button

![component_motor](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/component_motor.jpg)



LDRs

![component_ldr](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/component_ldr.jpg)



#### Design

Prototype (04/29)

![prototype](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/prototype.jpg)



Sample (04/30)

![model](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/model.jpg)



A finer case (05/03)

![model_case](/Users/yumingke/Documents/GitHub/DigitalElectronics_S18_Mingke/Final/images/model_case.jpg)



### Video

by 04/26, the operational project

[See video here](https://drive.google.com/open?id=1RIEyPjVpPg-VxG7BVmZRiryRxkMbb5bu)



### Program

[See code here](code/colordisc)
