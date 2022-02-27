# Abstract
This paper is about the designing of Current starved
ring oscillator using 28nm technology node. A total
of five stages of inverters will be used. The output
frequency of the oscillator is controlled by varying 
the control voltage. Waveforms are used to verify the
functionality of the circuitry.  
# Introduction
A VCO is an oscillator whose oscillation frequency is controlled by the value of
voltage provided at the input. In other words input voltage controls its frequency.
A VCO can be used in frequency and phase modulation techniques by applying 
modulating signal as a control voltage. It is also an integral part of Phase locked loop circuits.
The Ring Oscillator contains five number of stages with starved inverters. These are designed 
is a way that it forms a chain by connecting output of final stage to input of first stage
inverter. This configuration will produce an oscillatory output. This can be understood by
asserting that there is a small amount of delay that get introduced at every stage of inverter and then 
it is again fed back to the input stage which causes the oscillations in the circuit. 
The current starved technique is used so as to save power in comparison to push-pull inverters. 
From fig.1. we can see that the transistors M2 and M3 are working as an inverter whereas
transistor M5 and M6 are working as a current source. Here the drain currents ID4 and ID1
are controlled by control voltage provided at transistor M5. When an initial voltage is provided
at gate of M2 and M3, the output of inverter falls to 0. In this case, M1 is switched from saturation to triode region. 
Due to the current starved inverter, the current falls and the transistor M1 falls in deep triode
region which saves the power. The current sources, M1 and M4, limit the current available to the 
inverter, M2 and M3; in other words, the inverter is starved for current. The complete
circuit diagram is shown in fig.1.

![fig1](https://user-images.githubusercontent.com/100519853/155892918-1e1bef03-78da-48f3-a748-6b64f268d602.png)

                        fig.1. Rough schematic

# Schematic

![prince ckt](https://user-images.githubusercontent.com/100519853/155893395-4648cef5-a232-4244-9c56-498d54a17099.png)

                         fig.2.
             
 # Symbol
 
![symbol](https://user-images.githubusercontent.com/100519853/155893408-9f0e9519-add0-44e4-bbc4-7cb3c29b9382.png)

                         fig.3. 
                        
# Testbench Schematic For Current Starved VCO

![final schematic](https://user-images.githubusercontent.com/100519853/155893415-7331cede-31b6-4390-a71b-30bb12e92a00.png)

                          fig.4.
                          
 # Simulation Results 
 
 The output frequency for Vbias=0.35 volt comes out to be 1.56 GHz
 
![testresult0 35](https://user-images.githubusercontent.com/100519853/155895074-7cd0eb09-2748-4ac3-8c4a-7fa35de8908e.png)

                        fig.5. Waveform at Vbias=0.35v

The output frequency for Vbias=0.55 volt is 6.6 GHz

![testresult5 5](https://user-images.githubusercontent.com/100519853/155895078-f6b47d14-dfaa-4c6d-bef8-02191fe4da50.png)

                        fig.6. Waveform for Vbias=0.55v
                        
# Transistor Count

 NMOS=11
 
 PMOS=11
 
 Total transistors used=22
 
 # Netlist 
 
Kindly click [here](https://github.com/princepandey08/Current_Starved_VCO/blob/main/netist.txt) to see the netlist.



 
