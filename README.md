# COLORIMETER
## Introduction
A colorimeter is a laboratory device used to measure the absorbance of light at specific wavelengths in a given solution. Colorimetry is based on Beer-Lambert's law, which states that the amount of light absorbed by a colored solution is directly proportional to the solution's concentration and the length of the light path through it. When light passes through a sample solution, part of it is absorbed, while the remaining light is transmitted. By comparing the color intensity of a solute in the sample solution to that of a reference solution with a known solute concentration, we can estimate the concentration of the colored solute in the sample. Colorimeters are commonly used in fields such as water analysis, environmental analysis, and laboratory research.

Colorimeters, if accessible to households, could be used for practical applications like food quality control, water testing, and gardening. For instance, they could help ensure the freshness of fruits based on their color, test the purity of tap water, or analyze soil nutrients for home gardening. These applications could contribute to health, food safety, and environmental conservation efforts at a personal level.

## Overview of the Project

We are developing a colorimeter using an RGB LED to produce a spectrum of wavelengths by adjusting the intensity of the red, green, and blue LEDs individually. The emitted light passes through a solution sample in a cuvette positioned between the LED and a light-dependent resistor (LDR). LDR is a special resistor which creates variying voltage drop across it based on the intensity of incident light. The solution absorbs specific wavelengths based on the solute's concentration and nature of the solute. Unabsorbed light is incident on the LDR , where voltage variations are recorded to calculate the corresponding intensity of a particular wavelength and hence the intesity across the spectrum. The analysis is performed in a closed black box to eliminate the external light sources from disturbing the analysis. A Zero Analysis is performed with only the pure solvent (e.g., distilled water), prior to performing actual analysis by placing the sample of the solute. Then the difference between the actual analysis and zero analysis is taken. This significantly reduces the the external noise from other light sources and defects in the RGB leds which do not produce the exact wavelength.

![Components of a Colorimter](https://github.com/lightningbolt0827/ShreyasM-TusharM_RISC_hai_tho_ISHK_hai/assets/109969895/23a712fa-ae34-4a20-b27b-0ec177968f86)

The wavelength and light intensity of the light are then displayed on a 4-bit 7-segment display. To efficiently transfer data to the display unit and minimize the number of pins required, we are using a Serial-In-Parallel-Out (SIPO) shift register.

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




