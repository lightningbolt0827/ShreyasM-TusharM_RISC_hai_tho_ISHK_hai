# Colorimeter
## Introduction
A colorimeter is a laboratory device used to measure the absorbance of light at specific wavelengths in a given solution. Colorimetry is based on Beer-Lambert's law, which states that the amount of light absorbed by a colored solution is directly proportional to the solution's concentration and the length of the light path through it. When light passes through a sample solution, part of it is absorbed, while the remaining light is transmitted. By comparing the color intensity of a solute in the sample solution to that of a reference solution with a known solute concentration, we can estimate the concentration of the colored solute in the sample. Colorimeters are commonly used in fields such as water analysis, environmental analysis, and laboratory research.

Colorimeters, if accessible to households, could be used for practical applications like food quality control, water testing, and gardening. For instance, they could help ensure the freshness of fruits based on their color, test the purity of tap water, or analyze soil nutrients for home gardening. These applications could contribute to health, food safety, and environmental conservation efforts at a personal level.

## Overview of the Project
![Components of a Colorimter](https://github.com/lightningbolt0827/ShreyasM-TusharM_RISC_hai_tho_ISHK_hai/assets/109969895/23a712fa-ae34-4a20-b27b-0ec177968f86)


## Components Required

| Component | Quantity |
| ------------- | :-------------: |
| VSD Squadron Mini Board  | 1 |
| RGB LED (Common Cathode)  | 1  |
| 1.1 KΩ Resistor | 5 |
| 11 KΩ Resistor | 1|
| Light Dependent Resistor | 1 |
| 4 Bit Seven Segment Display | 1 |
| 74HC595 IC | 1 |
| Push Button | 1 |

## Circuit Connection Diagram

![Colorimeter_Circuit](https://github.com/lightningbolt0827/ShreyasM-TusharM_RISC_hai_tho_ISHK_hai/assets/109969895/67274c3d-f127-4e48-a6ae-a681b33005e1)


## Tables for Pin connection

| VSD Squadron Mini  | 74HC595 |
| ------------- | :-------------: |
| 3.3 V | Pin 16 (Vcc) and Pin 10 (~Master Reset) |
| GND | Pin 8 (GND) and Pin 13 (~Output Enable) |
| PC0 | Pin 11 (Clock) |
| PC1 | Pin 12 (Latch Pin) |
| PC2 | Pin 14 (Serial Data In) |

| VSD Squadron Mini  | 4 Bit Seven Segment Display |
| ------------- | :-------------: |
| PC3 | D1 |
| PC4 | D2 |
| PC5 | D3 |
| PC6 | D4 |

| VSD Squadron Mini  | RGB LED |
| ------------- | :-------------: |
| PD1 | Red |
| PD3 | Green |
| PD2 | Blue |
| GND | Common Cathode |

| VSD Squadron Mini  | Others |
| ------------- | :-------------: |
| PD0 | Push Button (Signal)|
| PA1 | LDR (Signal) |
| GND | Push Button (GND) and LDR (GND) |




