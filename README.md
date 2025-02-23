# BAE305-SP25-Lab4
# Laboratory Report for Lab 4 of BAE305 Spring 2025
# Lab 4 – Go Big : Operational Amplifiers
* By: Abby Phillips and Audrey Suit
* Submitted: February 24th, 2025

# Summary


# Materials

•	A Bread Board
•	Resistors: 1 kΩ, 4.7 kΩ, 8.2 kΩ, 22 kΩ, two 68 kΩ, 220 kΩ, 330 kΩ, 1.5 MΩ
•	Capacitors: 1nF and 100 nF
•	An LM741 Op Amp
•	A 10 kΩ trimmer potentiometer


# Assembly Procedures

### Part 1: Limits of Op Amps



### Part 2 : Op Amps and Frequency Response


# Test Equipment
1. Two DC Power Supplies
2. Fluke Digital Multimeter
3. Function Generator
4. Oscilloscope

# Test Procedures

## Part 1: Limits of Op Amps
### Step 1: Construct the Unity Gain Inverting Op Amp Circuit
1. Assemble the inverting amplifier circuit as shown in the lab manual.
2. Adjust the potentiometer to change input voltage (Vi) from -15V to +15V.
3. Measure and record output voltage (Vo) for at least nine different input voltages.
4.  Plot Vo vs. Vi data, comparing experimental values to theoretical expectations.

### Step 2: Construct the Moderate Gain Inverting Op Amp Circuit
1. Assemble the circuit as per Figure 3 in the lab manual.
2. Set the function generator to 100mV and 2 kHz.
3. Connect the oscilloscope: Channel 1 to Vi, Channel 2 to Vo.
4. Measure and record Vo, then calculate gain.
5. Compare measured gain with theoretical gain.

### Step 3: Constructing the High-Gain Inverting Op Amp Circuit
1. Assemble the circuit as per Figure 4 in the lab manual.
2. Set the function generator to 10mV and 2 kHz.
3. Observe the waveform on the oscilloscope and compare input and output signals.
4. Measure and record the gain of the circuit.
5. Compare theoretical vs. experimental gains for each circuit.
6. Discuss the maximum output voltage limits of Op Amps.
7. Evaluate symmetry of LM741 Op Amp performance in positive and negative regions.

## Part 2: Op Amps and Frequency Response

### Step 1: Construct a Voltage Follower
1. Assemble the voltage follower circuit as per Figure 5.
2. Set the function generator to 1V amplitude and 2 kHz.
3. Measure and compare Vi and Vo.
4. Increase frequency until performance degradation is observed; record the frequency limit.
5. Estimate the gain of the circuit.

### Step 2: Construct an Integrating Op Amp Circuit
1. Assemble the circuit as per Figure 6.
2. Set the function generator to 1Vp-p and 4 kHz.
3. Observe and document output waveforms for sine, square, and triangle wave inputs.
4. Change voltage and frequency, noting changes in waveform characteristics.

### Step 3: Construct a Differentiating Op Amp Circuit
1. Assemble the circuit as per Figure 7.
2. Set the function generator to 2Vp-p and 1 kHz.
3. Observe and document output waveforms for sine, square, and triangle wave inputs.
4. Change voltage and frequency, noting changes in waveform characteristics.
5. Did the circuits perform the expected mathematical operations?
6. Compare experimental output waveforms to theoretical derivatives/integrals.
7. Explain deviations in expected performance.

# Test Results


**Resistor Values Table**  
|Expected Value (Ω) | Measured Value (Ω) | Within Tolerance |
|-------------------|--------------------|--------------|
| 2200               | 2175           | yes|
|8200|8080| no|
|4700|4690|yes|
150000 |	147400 |yes|
68000 |	66600 |yes|
270000 |	266500 |yes|
1000 |	993 |yes|
1500000 |	14830000 |yes|
22 |	22.1 |yes|
33000 |	33340 |yes|
6800 |	67500 |yes|
22000 |	21640 |yes|

<p align="left"><em>Table 1: Measured, real values of the resistors used in the lab. The 8200 Ω resistor is not in tolerance, all other resistors are. </em></p>

**Capacitor Values Table**  
|Expected Value  | Measured Value  | Within Tolerance |
|-------------------|--------------------|--------------|
|.104 microF |	.104 microF |
|1 nF	| 1.44 nF|

<p align="left"><em>Table 2: Measured, real values of the capacitors used in the lab. </em></p>


### Part 1: Limits of Op Amps

**Vo vs. Vin for an Unity Gain Inverting Op Amp Circuit**  
|Vi  | Vo  | 
|-------------------|--------------------|
|-15 |	-0.265 |
|-14	| 0.222|
|-12|	1.202|
|-5	|4.66|
|0|	7.15|
|5	|9.63|
|12	|13.1|
|14	|14.13|
|15	|14.74|

<p align="left"><em>Table 3: Vo vs. Vi data collected by adjusting the potentiometer to change the input voltage. It is important to note we did not record the actual values for Vin and were unable to set the exact voltage each time. All values were within .1V of the recorded Vin. If we were to repeat the experiement, we would record experimental Vin values. </em></p>

**Gain of a Moderate Gain Op Amp Circuit**
|  |  Value  | |Value |
|-------------------|--------------------|--------------|--------------|
|Vin |90mV	 |Rin|8.2 kΩ|
|Vo |	3.36V |Rf|330 kΩ|
|Measured Gain (Vo/Vin) |	37.3 |Theoretical Gain (Rf/Rin)|40.24|

**Gain of a High Gain Op Amp Circuit**
|  |  Value  | |Value |
|-------------------|--------------------|--------------|--------------|
|Vin |9.6 mV	 |Rin|1 kΩ|
|Vo |	3.64V |Rf|1.5 MΩ|
|Measured Gain (Vo/Vin) |	379 |Theoretical Gain (Rf/Rin)|1500|

### Part 2: Op Amps and Frequency Response

**Measured Values of a Voltage Follower Op Amp Circuit**
|  |  Value  |
|-------------------|--------------------|
|Vin |431 mV	 |
|Vo |	440 mV |
|Measured Gain (Vo/Vin) |	1.2 |
|Frequency Limit| 8.4 kHz|

Note: output has low resistance

**Waveforms for Integration Op Amp Circuit**



**Waveforms for Differentiating Op Amp Circuit**



# Discussion


# Conclusion

