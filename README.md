# BAE305-SP25-Lab4
# Laboratory Report for Lab 4 of BAE305 Spring 2025
# Lab 4 – Go Big : Operational Amplifiers
* By: Abby Phillips and Audrey Suit
* Submitted: February 24th, 2025

# Summary

The goal of this lab is to learn how to use operational amplifiers (Op Amps) to build and analyze various signal conditioning circuits. We constructed and tested multiple configurations using an LM741 Op Amp, including a unity gain inverting circuit, moderate and high gain inverting amplifiers, a voltage follower, and both integrating and differentiating circuits. We used a function generator, digital multimeter, and oscilloscope to measure key parameters such as gain, voltage limits, and frequency response. First, we varied the input voltage in the unity gain circuit to observe the saturation points and verify the expected behavior. Next, we built moderate and high gain configurations to compare measured gains with theoretical predictions, noting slight discrepancies due to component tolerances and experimental limitations. Finally, we explored frequency response with a voltage follower and examined the mathematical operations of integration and differentiation on various waveforms. By the end of the lab, we had a better understanding of op amp performance, including practical limitations in gain and output voltage swing, as well as the importance of accurate component measurements in achieving reliable circuit behavior. Most measured values were within expected ranges, confirming the effectiveness of the LM741 in these applications.


# Materials

•	A Bread Board
•	Resistors: 1 kΩ, 4.7 kΩ, 8.2 kΩ, 22 kΩ, two 68 kΩ, 220 kΩ, 330 kΩ, 1.5 MΩ
•	Capacitors: 1nF and 100 nF
•	An LM741 Op Amp
•	A 10 kΩ trimmer potentiometer


# Assembly Procedures

### Part 1: Limits of Op Amps

Using the Fluke digital multimeter, we measured the actual resistance of the 1 kΩ, 4.7 kΩ, 8.2 kΩ, 22 kΩ, 68 kΩ, 220 kΩ, 330 kΩ and 1.5 MΩ resistors by attaching the multimeter probes to their terminals with alligator clips. The labeled resistance was verified using the resistor color code. 

This lab revolves around the usage of operational amplifiers, so below is Figure 1.0, a diagram of the 8-pin DIP op amp chips that we used. While building each circuit, we ensured that each component corresponded with the correct pin on the op amp.

![image](https://github.com/user-attachments/assets/05b03a64-81e7-4f68-b8f2-3b5e9b0a5053)


After verifying the resistor values, we proceeded to construct the unity gain inverting op amp circuit illustrated in Figure 1.1 and 1.2. All circuits, including this one, were constructed on a standard prototyping breadboard.

![image](https://github.com/user-attachments/assets/6185be82-3aab-4372-a025-f6e5277a7627)

After taking measurements of Circuit 1, as detailed in the Test Procedures section of this lab report, we built the moderate gain inverting op amp circuit shown below in Figures 2.1 and 2.2. 

![image](https://github.com/user-attachments/assets/78fe7f31-def2-4097-b7f1-6aee8bf423c4)

Shown also in Figure 2.2 is how we connected the oscilloscope. To create two waves, we plugged two oscilloscope probes. Both probes had their ground leads connected to ground via the resistor in the ground row, which is being used like a wire in this circumstance. The signal lead of one probe was attached to the Vin side of the 8.2kOhm resistor. The signal lead of the other probe was attached the the Vout side of the 330 kOhm resistor.

After taking measurements of Circuit 2, described in the Test Procedures, we built the high-gain inverting op amp circuit, seen in Figure 3.1 below. The change involved only the resistors, which we switched out for 1kOhm and 1.5MOhm resistors. Measurements of Circuit 3 were taken following the build, see Test Procedures below.

![image](https://github.com/user-attachments/assets/4db4593f-8599-411d-9f14-5527de8d4f5a)

### Part 2 : Op Amps and Frequency Response

We began this section by building a voltage follower, seen below in Figure 4.1. Going from the previous circuit, this required us to simply replace the 1kOhm resistor with a 68kOhm one, replace the 1.5 MOhm resistor with a wire, and disconnect the op amp from ground.

![image](https://github.com/user-attachments/assets/f10a3ca6-9338-4d5f-be54-72dc7ad2674f)

Following measurements of this Circuit 4, outlined in the Test Procedures, we built an integrating op amp circuit. This is seen below in Figures 5.1 and 5.2.

![image](https://github.com/user-attachments/assets/7e8e48ab-f539-4625-bf5e-3d6c1540c478)

Measurements of Circuit 5 were taken, further described in the Test Procedures, and then we built a differentiating op amp circuit. This circuit is shown in Figure 6.1 below.

![image](https://github.com/user-attachments/assets/6f61034e-118b-441b-a431-3666e224b18b)

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
4. Plot Vo vs. Vi data, comparing experimental values to theoretical expectations.

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

<p align="left"><em>Table 4: </em></p>

**Gain of a High Gain Op Amp Circuit**
|  |  Value  | |Value |
|-------------------|--------------------|--------------|--------------|
|Vin |9.6 mV	 |Rin|1 kΩ|
|Vo |	3.64V |Rf|1.5 MΩ|
|Measured Gain (Vo/Vin) |	379 |Theoretical Gain (Rf/Rin)|1500|

<p align="left"><em>Table 5: </em></p>

### Part 2: Op Amps and Frequency Response

**Measured Values of a Voltage Follower Op Amp Circuit**
|  |  Value  |
|-------------------|--------------------|
|Vin |431 mV	 |
|Vo |	440 mV |
|Measured Gain (Vo/Vin) |	1.2 |
|Frequency Limit| 8.4 kHz|

<p align="left"><em>Table 6:  </em></p>

Note: output has low resistance

**Waveforms for Integration Op Amp Circuit**
| Sine | Square   | Triangle|
|-------------------|--------------------|--------------------|
|![image](https://github.com/user-attachments/assets/7330c0d0-6ddc-4d73-bc8a-2e7ad42ba50a) |![image](https://github.com/user-attachments/assets/74f72ae0-b53b-4423-a9f4-27b591c39cd7)|![image](https://github.com/user-attachments/assets/4662b914-4dd0-418b-91cf-3879ca0d6f7f)|

<p align="left"><em>Table 7:  </em></p>




**Waveforms for Integration Op Amp Circuit with Increased Frequency**
|Sine |Square|
|--------------------|--------------------|
|![image](https://github.com/user-attachments/assets/903a2aa2-4176-4598-8f80-3a0b3f83622e) | ![image](https://github.com/user-attachments/assets/00a8bee6-1515-4eca-8303-839791280a9b)|

<p align="left"><em>Table 8:  </em></p>

**Waveforms for Differentiating Op Amp Circuit**
| Sine | Square   | Triangle|
|-------------------|--------------------|--------------------|
|![image](https://github.com/user-attachments/assets/992ecd7e-4d28-4c22-b60b-87689031c78e) |![image](https://github.com/user-attachments/assets/0ad94e7c-cd8c-416b-81f8-2749896856eb) |![image](https://github.com/user-attachments/assets/f2be9c05-f5df-41ea-935b-ea1ebeac8a82)|

<p align="left"><em>Table 9:  </em></p>

# Discussion


# Conclusion
