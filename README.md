![Microchip logo](images/microchip.png)
# Getting started with Mindi® simulation and PIC16F171XX microcontrollers

**Note : Currently, this repository contains mindi model of PIC18-Q41 family's OPAMP module. Mindi model of PIC16F171XX family's OPAMP module will be available soon.**

This guide will get you up and running with simulating the analog OPAMP module in PIC16F171XX family devices using the Mindi simulation tool. For more information about getting started with and using the MPLAB Mindi Analog Simulator please refer to the following resources:

- [Using the MPLAB Mindi Analog Simulator with the 8-Bit Operational Amplifier Module Technical Brief](https://ww1.microchip.com/downloads/en/DeviceDoc/Using-the-MPLAB-Mindi-Analog-Simulator-with-the-8-Bit-Operational-Amplifier-Module-90003293A.pdf)
- [Microchip Developer - Introduction to MPLAB Mindi Analog Simulator](https://microchipdeveloper.com/mindi:mindi-analog-simulator-introduction)
- [Getting Started with the MPLAB Mindi Analog Simulator Document](http://ww1.microchip.com/downloads/en/DeviceDoc/Getting-Started-MPLAB-Mindi-Analog-Simulator-DS50002564B.pdf)

## Configuration: Unity Gain Buffer (Voltage Follower)
A unity gain buffer is an opamp configuration in which the output voltage tracks the input voltage, also known as a voltage follower.

![Voltage Follower](images/configuration.png)

### Mindi Simulation
![Mindi](images/mplab-mindi-analog-simulator.png)

Download and open the follower **Mindi schematic [here](https://github.com/microchip-pic-avr-examples/pic16f171-opamp-mindi-unity-gain-buffer/releases/latest)**. Press the _play_ button to simulate with an example stimulus source.

### Adjustment Options
A voltage follower has no adjustable resistor values.

### Updating composer fields
Once the desired result has been verified with Mindi simulation, the corrected values should be moved back into MCC by copying resistor values across to the composer of your preference.

### Don't have Mindi?
You can download and install [Mindi simulation tool](https://www.microchip.com/mplab/mplab-mindi), or use another SPICE simulator of your own preference. For use with different simulators, a plain spice model can be found in "Opamp_PIC18_Q41.txt" to replace the mindi-optimized "Opamp_PIC18_Q41.lb "
