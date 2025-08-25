# Schmitt Trigger Using Op-Amp (UA741)

## Overview
This project is about designing and simulating a Schmitt trigger using a UA741 op-amp in LTSpice. The main idea was to see how hysteresis works when a triangular/pulse signal is applied and how the output switches cleanly between two voltage levels.

## Circuit Details
- UA741 op-amp (SPICE model included)  
- R1 = 10kΩ  
- R2 = 40kΩ  
- Input: Pulse signal (-3V to +3V, 1ms rise/fall, 2ms period)  
- Power supply: ±12V
<img width="1920" height="1080" alt="Schmitt_Trigger" src="https://github.com/user-attachments/assets/ec71d82f-f8dc-48b6-bec3-340aecc917dc" />

The non-inverting input is connected to ground through R1 and to the output via R2 to create positive feedback. The inverting input is connected to the pulse source. Output is taken from the op-amp’s output pin.

## Simulation
- Transient analysis  
- Stop time: 3 ms  
- Observed input vs output to check hysteresis behavior  

## Observations
- Output switched between about -10V and +10V  
- Switching happened around ±2V thresholds  
- Clear hysteresis was visible, confirming proper Schmitt trigger action  

## Files
- All LTSpice circuit files are in the folder Circuit Files
- All images are in the folder Images

## Conclusion
The Schmitt trigger worked as expected. The hysteresis created stable switching thresholds, which is useful for noise immunity and reliable digital interfacing.
