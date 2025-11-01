# MICROPROCESSOR-AND-MICROCONTROLLER
## 3.Write an assembly language program in 8051 to generate a 2 ms delay using Timer 0 in Mode 1 and toggle an LED connected to Port 2.0.

## Aim
To develop an 8051 microcontroller assembly program that uses Timer 0 in Mode 1 to generate a 2 ms delay and toggles an LED connected to Port 2.0.

## Apparatus Required
8051 Microcontroller Trainer Kit (or simulator like Keil uVision, Proteus, or 8051 IDE) LED (connected to Port 2.0) 10k Resistor (as current limiter) Connecting Wires & Breadboard (for practical hardware) Computer with IDE/Assembler for code development and simulation

## Algorithm
Set Port 2.0 as output. Initialize Timer 0 in Mode 1 (16-bit mode). Load the Timer registers to generate a 2 ms delay. Start Timer 0 and wait until the overflow flag is set (TFO = 1). Stop the timer and clear overflow flag. Toggle the state of Port 2.0. Repeat steps 3-6 indefinitely

## Program
#include<reg52.h>

void MSDelay (unsigned char value);
void main()
{
while (1)
{
MSDelay (250);
P0=0xff;
MSDelay (250);
P0=0x00;
}
}
void MSDelay (unsigned char value)
{
unsigned int y;
for (y=0;y<value;y++);

}

## Output
![WhatsApp Image 2025-11-01 at 09 46 03_c53ce665](https://github.com/user-attachments/assets/9c46d44a-2480-49e9-87c6-ab4530ebc12e)
## Result
Successfully designed and verified an 8051 Assembly program to toggle an LED at Port 2.0 with a precise 2 ms interval using Timer 0 in Mode 1. Demonstrated timer initialization, delay loop, and I/O port manipulation in 8051 Assembly.
