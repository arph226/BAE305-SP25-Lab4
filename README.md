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
<p align="left"><em>Figure 1.0: Schematic of 8-pin DIP Operational Amplifier Chip. </em></p>

After verifying the resistor values, we proceeded to construct the unity gain inverting op amp circuit illustrated in Figure 1.1 and 1.2. All circuits, including this one, were constructed on a standard prototyping breadboard. Note the 10 kOhm resistor in the schematic refers to the potentiometer. 

![image](https://github.com/user-attachments/assets/6185be82-3aab-4372-a025-f6e5277a7627)
<p align="left"><em>Figure 1.1: Schematic of Circuit 1. A unity gain inverting op amp. </em></p>

![image](https://github.com/user-attachments/assets/236b8c2d-8f7e-43d6-9ae2-aefb05901ef2)
<p align="left"><em>Figure 1.2: Image of Circuit 1. A unity gain inverting op amp, with a potentiometer being the 10 kOhm resistor. </em></p>

After taking measurements of Circuit 1, as detailed in the Test Procedures section of this lab report, we built the moderate gain inverting op amp circuit shown below in Figures 2.1 and 2.2. 

![image](https://github.com/user-attachments/assets/78fe7f31-def2-4097-b7f1-6aee8bf423c4)
<p align="left"><em>Figure 2.1: Schematic of Circuit 2. A moderate gain inverting op amp. </em></p>

Shown also in Figure 2.2 is how we connected the oscilloscope. To create two waves, we plugged two oscilloscope probes. Both probes had their ground leads connected to ground via the resistor in the ground row, which is being used like a wire in this circumstance. The signal lead of one probe was attached to the Vin side of the 8.2kOhm resistor. The signal lead of the other probe was attached the the Vout side of the 330 kOhm resistor.

![image](https://github.com/user-attachments/assets/a9d4a963-5dd3-4d05-9750-131b95c64250)
<p align="left"><em>Figure 2.1: Image of Circuit 2. A moderate gain inverting op amp and oscilloscope probes connected to Vin and Vout. </em></p>

After taking measurements of Circuit 2, described in the Test Procedures, we built the high-gain inverting op amp circuit, seen in Figure 3.1 below. The change involved only the resistors, which we switched out for 1kOhm and 1.5MOhm resistors. Measurements of Circuit 3 were taken following the build, see Test Procedures below.

![image](https://github.com/user-attachments/assets/129875c6-a08c-440e-828a-d060bb7763fa)
<p align="left"><em>Figure 3.1: Schematic of Circuit 3. A high-gain inverting op amp circuit. </em></p>

### Part 2: Op Amps and Frequency Response

We began this section by building a voltage follower, as seen below in Figure 4.1. Going from the previous circuit, this required us to simply replace the 1kOhm resistor with a 68kOhm one, replace the 1.5 MOhm resistor with a wire, and disconnect the op amp from ground.

![image](https://github.com/user-attachments/assets/57bd67e6-f1af-410f-93e0-d7aed469f7d0) 
<p align="left"><em>Figure 4.1: Schematic of Circuit 4. A voltage follower op amp circuit. </em></p>

Following measurements of Circuit 4, outlined in the Test Procedures, we built an integrating op amp circuit. This is seen below in Figure 5.1. 

![image](https://github.com/user-attachments/assets/92a684cf-5c13-4265-abb9-5d773debd935)
<p align="left"><em>Figure 5.1: Schematic of Circuit 5. An integrating op amp circuit. </em></p>

Measurements of Circuit 5 were taken, further described in the Test Procedures, and then we built a differentiating op amp circuit. This circuit is shown in Figures 6.1 and 6.2 below.

![image](https://github.com/user-attachments/assets/6bc8e337-9b93-4a02-b055-684fbb1b7dfa)
<p align="left"><em>Figure 6.1: Schematic of Circuit 6. A differentiating op amp circuit. </em></p>

![image](https://github.com/user-attachments/assets/f5198fe8-8696-4725-b982-2273ee4a1682)
<p align="left"><em>Figure 6.2: Image of Circuit 1. A differentiating op amp circuit. </em></p>


# Test Equipment
1. Two DC Power Supplies
2. Fluke Digital Multimeter
3. Function Generator
4. Oscilloscope

# Test Procedures

NOTE: For all test procedures, positive and negative power voltages were created by using 2 power supplies. We checked polarity of the power supplies before connecting the op-amps. We also measured all of the resistors and capacitors in the lab to make sure they were in tolerance as shown in Table 1 and 2.

## Part 1: Limits of Op Amps
### Step 1: Construct the Unity Gain Inverting Op Amp Circuit
1. Assemble the inverting amplifier circuit as shown in Figure 1.1. Drive the voltage divider with positive and negative voltage supplies
2. Adjust the potentiometer to change input voltage (Vi) from -15V to +15V. We did not record exact input values, but it is recommended you do.
3. We measured and recorded output voltage (Vo) for at least nine different input voltages in the range listed above in Table 3.
4. Plot Vo vs. Vi data, comparing experimental values to theoretical expectations.

### Step 2: Construct the Moderate Gain Inverting Op Amp Circuit
1. Assemble the circuit as per Figure 2.1 and 2.2 in the assembly procedures.
2. Set the function generator to 100mV and 2 kHz.
3. Connect the oscilloscope: Channel 1 to Vi, Channel 2 to Vo.
4. Measure and record Vo and Vin by using the measurment feature on the oscilloscope. We used the measurement tool for more precise values. 
5. Compare measured gain with theoretical gain calculated with the measured resistance values in Table 4.

### Step 3: Constructing the High-Gain Inverting Op Amp Circuit
1. Assemble the circuit as per Figure 3.1 in the assembly procedures.
2. Set the function generator to 10mV and 2 kHz.
3. Observe the waveform on the oscilloscope with channel 1 connected to Vi and channel 2 to Vo. We compared input and output signals to look at the symmetry of the waveform.
4. We calculated experimental gain from measured Vo and Vin values using the same process as above and recorded in Table 5
5. We then compared theoretical vs. experimental gains for each circuit using measured resistance values.

## Part 2: Op Amps and Frequency Response

### Step 1: Construct a Voltage Follower
1. Assemble the voltage follower circuit as per Figure 4.1.
2. Set the function generator to 1V amplitude and 2 kHz.
3. Check to confirm input and output voltage were the same by looking at max measurment values on the oscilloscope
4. Measure and compare Vi and Vo and calculate gain.
5. To find the frequency limit we increased frequency until performance degradation is observed and recorded the limit in Table 6

### Step 2: Construct an Integrating Op Amp Circuit
1. Assemble the circuit as per Figure 5.1.
2. Set the function generator to 1Vp-p and 4 kHz.
3. Change the wave forms between sine, square, and triangular. Be sure to take pictures of the waveforms for reference. In order to get a good image we adjusted the sec/div knobs and other values until we created a clear image with both waves in range.
5. Change voltage and frequency, noting changes in waveform characteristics. Take pictures of the results

### Step 3: Construct a Differentiating Op Amp Circuit
1. Assemble the circuit as per Figure 6.1 and 6.2.
2. Set the function generator to 2Vp-p and 1 kHz.
3. Observe and document output waveforms for sine, square, and triangle wave inputs as described in Step 2.
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

**Vo vs. Vin for a Unity Gain Inverting Op Amp Circuit**  
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

<p align="left"><em>Table 3: Vo vs. Vi data collected by adjusting the potentiometer to change the input voltage. It is important to note we did not record the actual values for Vin and were unable to set the exact voltage each time. All values were within .1V of the recorded Vin. If we were to repeat the experiment, we would record experimental Vin values. As shown, as the input voltage (Vi) increases from -15 to 15, the output voltage (Vo) also increases. This aligns with the expected behavior of an inverting op amp circuit, however, it seems like there are some symmetry issues in the data. According to the gain equation Vo= -(Rf/Rin)Vi, the Vo value should be opposite the Vin value. For example, at Vi=-15V, Vo should be 15V. However, the resistance values are not equal due to tolerance in the resistors, which likely leads to some variation. This would not fully explain the non-symmetric variation, so there could be errors in the circuit's wiring. </em></p>

![image](https://github.com/user-attachments/assets/94a1e020-5850-4cae-a9e7-edd15270782f)
<p align="left"><em> Graph 1: Vo vs. Vi data collected by adjusting the potentiometer to change the input voltage as outlined in Table 3. As shown, Vo should be the inverse of Vo, however our measured values are slightly skewed which could be due to issues we were experiencing with out breadboard. </em></p>

**Gain of a Moderate Gain Op Amp Circuit**
|  |  Value  | |Value |
|-------------------|--------------------|--------------|--------------|
|Vin |90mV	 |Rin|8.2 kΩ|
|Vo |	3.36V |Rf|330 kΩ|
|Measured Gain (Vo/Vin) |	37.3 |Theoretical Gain (Rf/Rin)|40.24|

<p align="left"><em>Table 4: The measured and theoretical gain for a moderate gain inverting op amp circuit was calculated from measured Vin, Vo, Rin, and Rf values. It appears the experimental gain is slightly lower than the theoretical gain, but the values are still close to one another.</em></p>

**Gain of a High Gain Op Amp Circuit**
|  |  Value  | |Value |
|-------------------|--------------------|--------------|--------------|
|Vin |9.6 mV	 |Rin|1 kΩ|
|Vo |	3.64V |Rf|1.5 MΩ|
|Measured Gain (Vo/Vin) |	379 |Theoretical Gain (Rf/Rin)|1500|

<p align="left"><em>Table 5: The measured and theoretical gain for a high-gain inverting op amp circuit was calculated from measured Vin, Vo, Rin, and Rf values. It appears the experimental gain is much lower than the theoretical gain. This is due to issues with our function generator, which created non-symmetrical appearing waves. We were unable to determine the errors occurring in collaboration with Dr. Jarro, so we proceeded to the next step of the lab.</em></p>

### Part 2: Op Amps and Frequency Response

**Measured Values of a Voltage Follower Op Amp Circuit**
|  |  Value  |
|-------------------|--------------------|
|Vin |431 mV	 |
|Vo |	440 mV |
|Measured Gain (Vo/Vin) |	1.2 |
|Frequency Limit| 8.4 kHz|

<p align="left"><em>Table 6: The measured gain for a voltage follower op amp circuit was calculated from measured Vin and Vo values. It appears the measured gain is close to one, which is expected for a voltage follower in which Vo and Vi should be the same. The output of a voltage follower has very low resistance. When using the function generator, we found the frequency limit to be about 8.4 kHz. </em></p>

Note: output has low resistance

**Waveforms for Integration Op Amp Circuit**
| Sine | Square   | Triangle|
|-------------------|--------------------|--------------------|
|![image](https://github.com/user-attachments/assets/7330c0d0-6ddc-4d73-bc8a-2e7ad42ba50a) |![image](https://github.com/user-attachments/assets/74f72ae0-b53b-4423-a9f4-27b591c39cd7)|![image](https://github.com/user-attachments/assets/4662b914-4dd0-418b-91cf-3879ca0d6f7f)|

<p align="left"><em>Table 7: The input and output waveforms for an integrating op amp circuit for 4kHz, 1Vp-p, sine, square, and triangular waves. Integrating op amp circuits produce an output that is the integral of the input. In the images, the input is labeled in yellow, and the output is in blue. As shown in the images, the sine wave input yields a slight phase shifted output, the square wave input yields a slightly more triangular/trapezoidal output, and the triangular input yields a parabolic output. These results are as expected since the output is the integral of the input.  </em></p>



**Waveforms for Integration Op Amp Circuit with Increased Frequency**
|Sine |Square|
|--------------------|--------------------|
|![image](https://github.com/user-attachments/assets/903a2aa2-4176-4598-8f80-3a0b3f83622e) | ![image](https://github.com/user-attachments/assets/00a8bee6-1515-4eca-8303-839791280a9b)|

<p align="left"><em>Table 8: The input and output waveforms for an integrating op amp circuit for 4kHz, 1Vp-p, sine, square, and triangular waves after increasing frequency. As shown in the sine and square waveforms, when frequency increases, the amplitude of the output decreases. Additionally, when the frequency increases for the square wave input, the triangles in the output become steeper, even though the amplitude decreases.  </em></p>

**Waveforms for Differentiating Op Amp Circuit**
| Sine | Square   | Triangle|
|-------------------|--------------------|--------------------|
|![image](https://github.com/user-attachments/assets/992ecd7e-4d28-4c22-b60b-87689031c78e) |![image](https://github.com/user-attachments/assets/0ad94e7c-cd8c-416b-81f8-2749896856eb) |![image](https://github.com/user-attachments/assets/f2be9c05-f5df-41ea-935b-ea1ebeac8a82)|

<p align="left"><em>Table 9: The input and output waveforms for a differentiating op amp circuit for 1kHz, 2Vp-p, sine, square, and triangular waves. Differentiating op amp circuits produce an output that is the derivative of the input. In the images, the input is labeled in blue, and the output is in yellow. As shown in the images, the sine wave input yields a cosine wave, the square wave input yields a series of sharp peaks, and the triangular input yields a smooth curved waveform. The sine wave input should yield a cosine wave, the square wave should yield a series of sharp spikes, and the triangle wave should yield a square wave. The sine and square waves were as expected, but the triangle wave output was not square. That being said, this could be due to how the op-amp reacts to the change in slope creating a more smooth shape than the expected square. </em></p>


# Discussion

We faced some error due to malfunctions with our breadboard and function generator. However, we were still able to reach a general understanding of op amp functionality and possibilities for use in other purposes. Errors were supplemented by clarification from Carlos and research done following the conclusion of the lab. Both contributed to our understanding and the answering of the questions below.

Discussion Question 1: Compare the performance of each amplifier circuit to its expected theoretical performance regard to gain.

Gain should be infinite in an ideal op amp. The gain we saw with the moderate gain inverting op amp circuit was around expected theoretical performance.

Discussion Question 2: Comment on the limits of op amp circuits with respect to maximum output voltage.

Since op amp circuits are limited by their power supply rails, for the LM741, the maximum output voltage is typically a few volts less than the supply voltages. This means that regardless of the theoretical gain, the output cannot exceed these rail voltages. In reality, as the input signal increases, the op amp will eventually saturate and stall the output when it reaches these limits. Additionally, factors like internal voltage drops and load conditions can further limit the maximum output voltage.

Discussion Question 3: Are the LM741 op amps symmetric i.e. does the positive voltage performance equal the negative voltage performance?

Symmetry was observed for the moderate gain inverting op amp, but not the high-gain inverting op amp. This was due to errors in the function generator. Both op amps should be produce symmetric performance.

Discussion Question 4: Did the integrating and differentiating circuits perform the mathematical operations expected?

Yes, we know the derivative of a sine wave is a cosine wave, a derivative of a triangle wave is a square wave, and the derivative of a square wave is a triangle wave. When we set the function generator to each of these wave types, the other wave reflected the correctly corresponding derivative.


# Conclusion

This lab was focused on the exploration and analysis of operational amplifiers (op amps) in constructing and testing various signal conditioning circuits. We utilized the LM741 op amp and built several configurations, including unity gain inverting, moderate gain inverting, high-gain inverting, voltage follower, integrating, and differentiating circuits. Using a function generator, digital multimeter, and oscilloscope, we measured and compared parameters such as gain, voltage limits, and frequency response. 

Our results indicated that while most circuits performed as expected, some variations between theoretical and experimental values were observed, mainly due to tolerances in component values and experimental limitations. The moderate gain circuits closely matched theoretical predictions, while the high-gain configurations displayed some discrepancies, likely due to equipment issues. The voltage follower circuit exhibited near-unity gain up to a frequency limit of around 8.4 kHz. Finally, the integrating and differentiating circuits successfully performed their intended mathematical operations, such as integration and differentiation, with minor observed deviations. 

By the end of this lab, we gained a deeper understanding of how op amps function in different configurations and the practical limitations these op amps face with respect to gain, voltage output, and frequency range. This hands-on experience reinforced the importance of accurate component measurements and provided insights into real-world applications of op amps.
