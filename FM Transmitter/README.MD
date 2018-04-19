# FM Transmitter Used In Animal Tracking
An animal tracking system is designed, where an FM Transmitter is attached to an animal for tracking. The transmitter is printed on a PCB.

The following circuit is designed in ADS:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterCircuitADSNominalVal.PNG "FM Transmitter Circuit on ADS")

Then drawn in Audodesk Eagle:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterCircuit.PNG "FM Transmitter Circuit on Eagle")

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterEagle.PNG "FM Transmitter on Eagle")

The circuit is milled onto a double sided copper PCB:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterPCB.jpg "FM Transmitter on PCB")

Front of PCB:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterPCBFront.jpg "PCB Front")

The closest available components are sottered onto board for testing.

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterPrototype.jpg "Low Power FM Transmitter")

The first measurements are taken by powering the transimitter, and testing the circuit's output signal
using a spectrum analyzer. The signal seems to stay at around 260 MHz, zooming in shows oscillations 
of +/- 10Mhz.

The transmitter is then taken to a lab equipped with a PicoScope and TIMS equipement. Retrofitting an antenna
to the input of the PicoScope input, and then powering the transmitter outputs the signal. 
The signal oscillates at around 260 MHz.
The next step will be to stabalize the signal and demodulate to test if sent tone is being properly modulated.
Suspect the signal will be distorted since the carrier frequency is oscillating at a bandwidth that is 
too large.

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterFirstResults.jpg "First Results")

Conclusions: The FM transmitter is tested using a spectrum analyzer, the signal has a carrier frequency of around 260 MHz, 
the signal oscillates between 250 MHz to 265 MHz. The carrier swing may be due to the board being too big, 
having the copper nodes too far apart, using unideal components.


