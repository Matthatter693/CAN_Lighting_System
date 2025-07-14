 # Vehicle Lighting System on LPC2129

 Lights are important in a vehicle just like how we all need some positive light in life! So here to solve that I implemented a lighting system which is made possible due to the CAN (Controller Area Network)
 present in LPC2129 a ARM7 based microcontroller. Here is a quick walkthrough to my design.

 ## Features
 - The switch controls for the light is implemented internally with external interrupts so achieving a higher response time compared to their polling based condition checks.
 - A full fletched CAN Bus is adhering with CAN 2.0A standard which is simple and efficient for the automotive control works.
 - The Decentralized setup with seperate ECU's is less prone to failure in times of malfunction.
 - Added UART support for effective debugging of frames in the serial terminal.
 - Drivers written from scratch that runs in a bare-metal setup without heavy dependence on external libraries.

## Setup

The entire code-base here is written in Keil Microvision 5 and the startup code is provided by the NXP semiconductors. Replications of this project can be done by cloning the repository and opening the files
in Keil. 

> **NOTE:** This implementation of Embedded-C code is targetted towards LPC2129 microcontroller. To run in the other it requires some slight modifications so refer your microcontroller datasheet accordingly
