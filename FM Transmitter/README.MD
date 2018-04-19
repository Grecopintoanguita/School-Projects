# FM Transmitter Used In Animal Tracking
An animal tracking device is designed using a low power FM Transmitter. The transmitter is printed on a PCB
and tested for frequency response.

The following circuit is designed in ADS to create a low power FM Transmitter:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterCircuitADSIdeal.PNG "FM Transmitter Circuit on ADS")

Then drawn in Audodesk Eagle:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterCircuit.PNG "FM Transmitter Circuit on Eagle")

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterEagle.PNG "FM Transmitter on Eagle")

The circuit is milled onto a double sided copper PCB:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterPCB.jpg "FM Transmitter PCB")

Front of PCB:

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterPCBFront.jpg "PCB Front")

The closest available components are soldered onto the board for testing.

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterPrototype.jpg "Low Power FM Transmitter")

The spectrum of the transmitter output is first measured using a Spectrum Analyzer.
The signal stays at around 260 MHz, zooming in shows oscillations of +/- 10Mhz.

The transmitter is then taken to a lab equipped with a PicoScope and TIMS equipement. 
An antenna is retrofitted to the input of the PicoScope.
The signal oscillates at around 260 MHz, corroborating the Spectrum Analyzer.

![alt text](https://github.com/Grecopintoanguita/School-Projects/blob/master/images/FMTransmitterFirstResults.jpg "First Results")

The signal resembles an AM signal more than an FM signal. The first step is to use a comparator to check if the
signal is indeed FM, if not, reevaluate circuit design.  I suspect that the signal will be distorted after 
demodulation, since the carrier frequency is oscillating in a relatively high bandwidth.

