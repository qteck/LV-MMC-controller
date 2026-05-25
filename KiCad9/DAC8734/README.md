# Data Acquisation
This is an isolated quad DAC board which can serve a variety of purposes, such as simple conversion of a digital signal into an analogue signal for monitoring purposes, but also as an instrumentation analogue switch.

The core of the board is the DAC8734. This chip cannot output high currents, but it is enough to drive some peripheral switching circuits that can boost power to trigger circuits that may be more power demanding, such as high-power MOSFETs for motor drives.

## Improvemenets: 
This chip has got very high versatility, and in reference to its application and the universality of this data acquisition system, the board would benefit from implementing switching options for the coaxial output, such as unipolar vs bipolar output and gain settings. This could be done through a series of small mechanical switches, jumpers or solder bridges.

### VMON ADC

The current solution for the monitoring of the outputs is a matter of compromise. The coaxial outputs are unipolar in order to have only positive voltage on the VMON pin that is fed into the ADC.

This limits the output options from bipolar and unipolar to unipolar only and should be addressed in the next iteration by scaling and level-shifting the VMON above GND level for bipolar outputs.


## Front Side 
![acquisation front](../../Images/acquisition_front.jpg)
## Back Side
![acquisation back](../../Images/acquisition_back.jpg)