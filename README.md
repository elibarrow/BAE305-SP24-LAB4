# Lab Report 4 - Go Big: Operational Amplifiers
Eli Barrow & Isaac Stevens

Feb. 8, 2024

## Summary of Lab ##


The purpose of the lab was to learn how to use operation amplifiers (Op-amps) to construct basic amplifiers and signal conditioning circuits and to discover the limitations of op-amps. To create this understanding, Lab 4, Part 1 designates creating a low, moderate, and high gain inverting op-amp circuit. This was accomplished by creating one inverting op-amp circuit and changing the resistors within the circuit. For the low gain circuit, the $V_i$ and $V_o$ were measured with DMM at changing voltage by adjusting the potentiometer, and for the other two circuits, the gain was calculated using a constant voltage and measured $V_i$ and $V_o$ from the DMM. Only for the low gain circuit was $R_i$ and $R_f$ measured with the DMM to calculate an expected gain from the resistance compared to the slope (gain) of the documented $V_i$ and $V_o$ from the changing voltage. By completing Part 1, our group gained a greater understanding of the limits of op-amp circuits.


Part 2 designates creating a voltage follower op-amp circuit and the gain was calculated using the measured $V_i$ and $V_o$ from the oscilloscope-generated functions of the two voltages. Next, an integration op-amp circuit was created and the gain was calculated using the measured $V_i$ and $V_o$ from the oscilloscope-generated functions of the two voltages. Lastly, a differentiating op-amp circuit was created and the gain was calculated using the measured $V_i$ and $V_o$ from the oscilloscope-generated functions of the two voltages. Creating these op-amp circuits gave us a better understanding of how different types of op-amps function and concluded Part 2 and therefore completed Lab 4.


### Lab Objective: Learn to use Op Amps, its circuits, and applications ###  



## Lab Assignment Specific Items ##

For Lab 4, the following materials are required:

• A Larger Breadboard 

• 2 Digital Multi-meter (DMM): Fluke 87

• 2 DC Power Supply: Global Specialties 1403

•	9 Resistors: 1 kΩ, 4.7 kΩ, 8.2 kΩ, two 68 kΩ, 150 kΩ, 270 kΩ, 330 kΩ, 1.5 MΩ

• 2	Capacitors: 1nF and 100 nF

• A Function Generator: Global Specialties 2001A

•	An LM741 Op Amp

•	A 1kΩ trimmer potentiometer

No code is required to complete Lab 4



## Part 1 - Limits of Op Amps ##

### Circuit 1 ###

We began this lab by constructing the unity gain inverting op amp circuit shown below.

<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%201.png>
</p>

We drove the voltage divider with the positive and negative voltage supplies from the DC Power Supply: Global Specialties 1403. We then collected $V_o$ and $V_i$ data by adjusting the potentiometer to change the input voltage. We collected 9 values that range from the negative and positive saturation points. 

Below is a picture of how the voltage values were measured during the lab with a table of the measured values:

<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Setup%20of%20Circuit.jpg width=100%>
</p>


 |Test Point|  $V_i$ (Volts)|  $V_o$ (Volts) |
|---|---|---|
|1|  -14.99 V | 14.23 V|
|2| -9.27 V  | 9.31 V|
|3|  -5.82 V | 5.86 V |
|4|  -1.763 V | 1.791 V|
|5|  0.190 V | -0.165 V |
|6|  1.598 V | -1.574 V|
|7|  5.000 V | -4.981 V|
|8|  10.03 V | -10.02 V |
|9|  14.98 V | -13.61 V|


After taking this data we prepared a graph that shows the lab data as scattered points and calculated the expected gain considering the resistor values in the circuit.

$R_f$ = 67.4 k&Omega;  
$R_i$ = 67.9 k&Omega;  
 Equation of the Gain = (-($R_f$)/($R_i$))  
 Expected Gain = -(67.4 k&Omega;)/(67.9 k&Omega;) = -0.993   
*The graph of our collected data is shown below* 

<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Gains%20Graph.png width=65%>
</p>

### Circuit 2 ###
 After completing the gain analysis for Circuit 1 we then moved on to analyze another circuit, which is shown below.

 <p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%202.png width=35%>
</p>

Below is how our group constructed Circuit 2 during the lab:

 <p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Example%20of%20Circuit%202.jpg width=75%>
</p>


After constructing this moderate gain op-amp circuit we connected the function generator to $V_i$ and used the oscilloscope to plot $V_i$ in channel 1 and $V_o$ in channel 2.

<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Moderate%20Gain.JPG width=35%>
</p>

 Using the O-scope we measured and calculated the gain of the circuit.  
Gain = -(10V)/(1V)  
Gain = -10V

### Circuit 3 ###

 After calculating the gain of the moderate gain op-amp circuit we moved on to build the high gain inverting op-amp circuit, which is shown below.

<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%203.png width=35%>
</p>

 After constructing this circuit we followed similar steps to those in part 2 to use the O-scope to calculate the gain of the circuit.

 <p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/High%20Gain.JPG width=35%>
</p>

 Gain = -(7.08 V)/(0.268 V)   
 Gain = -26.11 V

**Discussion Questions**
1. Compare the performance of each amplifier circuit to its expected theoretical performance with regard to gain.  

**Response:** The gain of the first amplifier circuit was -0.955 while the theoretical performance of a non-inverting op amplifier circuit is expected to be -1.

2. Comment on the limits of op-amp circuits with respect to maximum output voltage.

**Response:** Once the maximum output voltage is reached in the op-amp circuit, the op-amp reaches saturation and begins to output its maximum voltage instead of amplifying input voltage to output voltage exponentially.

4. Are the LM741 op-amps symmetric i.e. does the positive voltage performance equal the negative voltage performance?  

**Response:** The LM741 op-amps are symmetric and the positive voltage performance does equal the negative voltage performance for the first circuit until below -12V or above 12V which causes the $V_i$ to not equal $V_o$.

## Part 2 - Op Amps and frequency response ##


### Circuit 4 ###
We began part 2 of the lab by building the following voltage follower circuit.
<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%204.png width=35%>
</p>

Below is how our group constructed Circuit 4 during the lab:

 <p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Example%20of%20Circuit%204.jpg width=75%>
</p>

By using the O-scope and the function generator we were able to collect $V_i$ and $V_o$ data with those instruments. The data presented on the O-scope is shown below. 
<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Voltage%20Follower.JPG width=35%>
</p>

We then estimated the gain for this voltage follower circuit.  
Gain = (0.288 V)/(0.280 V) 
Gain = 1.03 V

Note: Since we were running low on time in the lab we did not connect the function generator to find out and record what the frequency limit was for the 741 op amp.     


### Circuit 5 ###

The next circuit that we built was an integrating op amp, the schematic for that circuit is shown below.
<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%205.png width=35%>
</p>

Below is how our group constructed Circuit 5 during the lab:

 <p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Example%20of%20Circuit%205.jpg width=75%>
</p>

Upon connecting the function generator to the circuit the O-scope showed the following input and output waveforms: 
<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Integrating.JPG width=35%>
</p>  
We then estimated the gain for this integrating op amp circuit. 

Gain = (0.232 V)/(0.600 V)              
Gain = 0.386 V        

Question: Change the voltage and frequency and note any differences.

**Response:** When changing the voltage, the input and output increase with increased voltage. When changing the frequency, the amplitude decreases when increasing the frequency.  





### Circuit 6 ###

The next circuit that we built was a differentiating op amp, the schematic for that circuit is shown below.
<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%206.png width=35%>
</p>  
 
Upon connecting the function generator to the circuit the O-scope showed the following input and output waveforms: 
<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Differentiating.JPG width=35%>
</p>  
We then estimated the gain for this integrating op amp circuit.  

Gain = (7.04 V)/(7.08 V)     
Gain = 0.994 V      

Question: Change the voltage and frequency and note any differences.

**Response:** When changing the voltage, the input and output increase with increased voltage. When changing the frequency, the amplitude decreases when increasing the frequency.


**Discussion Question: Did the integrating and differentiating circuits perform the mathematical operations expected? Explain.**  

The integrating and differentiating circuits performed the mathematical operations expected because for the integrating circuit, the input was a square and the output was a triangle with the integral of a square being a triangle. For the differentiating circuit, the input was a square and the output was a sloped line with the integral of a square being a slope.


## Conclusion of Lab 4 ##

The lab's outcome was using different op-amp circuits and measuring properties within the circuit such as voltage and resistance allowing the gain to be calculated from the op-amp. By calculating the gain of the circuit, we gain a better understanding of the behavior and limitations associated with different types of op-amp circuits. For Part 1 of the lab, by measuring the $V_i$ and $V_o$ using a DMM and changing the voltage for the low gain inverting op-amp circuit, we were able to graph $V_i$ over $V_o$ which gave us a gain (slope of the graph) using voltage of -0.955. When compared to the expected gain using resistance of -0.993, we can see that the $Gain_V$ > $Gain_R$.  This difference in gain demonstrates a property associated with real-life op-amps. This property is as $V_-$ approaches -15V or $V_+$ approaches 15V, the $V_i$ and $V_o$ do not equal each. While we assume op-amps to be ideal within the bounds of this class, op-amps in real life are limited by this property so the expected gain or ideal gain does not always equal the real gain especially when $V_-$ approaches -15V or $V_+$ approaches 15V.

In the moderate-gain and high-gain inverting op-amp circuit, $V_i$ and $V_o$ were measured using a DMM at a constant voltage to calculate the gain from the circuit. The gain for the moderate-gain inverting op-amp circuit was equal to -10 and the high-gain inverting op-amp circuit gain was equal to -26.11. By comparing the gain between all three circuits in Part 1, we were able to demonstrate as gain decreases (becomes more negative) in an inverting op-amp circuit, the difference between $V_i$ and $V_o$ increases and shows the effect an inverting op-amp has on the voltage associated within the circuit.

For Part 2 of the lab, three circuits were constructed: a voltage follower op-amp circuit, an integration op-amp circuit, and a differentiation op-amp circuit. The $V_i$ and $V_o$ were measured at a constant voltage, however, for Part 2, were measured using a function generator with the voltage function with respect to time being displayed on an oscilloscope. When measuring the $V_i$ and $V_o$ of the voltage follower op-amp circuit, the gain was calculated to be equal to 1.03 with the $V_i$ almost equally $V_o$ and both voltage functions being nearly identical. When measuring the $V_i$ and $V_o$ of the integration op-amp circuit, the gain was calculated to be equal to 0.368 with the $V_i$>$V_o$ and $V_o$ being triangular waves when compared to $V_i$'s square waves showing $V_o$ to be the integral of $V_i$. When measuring the $V_i$ and $V_o$ of the differentiating op-amp circuit, the gain was calculated to be equal to 0.994 with the $V_i$ almost equaling $V_o$ and $V_o$ being square waves this time while $V_i$'s waves were triangular showing $V_o$ to be the derivative of $V_i$.

By calculating the gain and displaying the $V_o$ and $V_o$ functions on the oscilloscope, we were able to demonstrate behaviors associated with these types of op-amps. The voltage follower op-amp circuit had $V_o$ following $V_i$ and almost being equal. The integration op-amp circuit had $V_o$ voltage function be the integral of $V_i$. Lastly, differentiating op-amp circuit had $V_o$ voltage function be the derivative of $V_i$. By using the function generator and oscilloscope to display trends in these types of op-amp circuits, our group was able to have a greater understanding of op-amp circuits.

Lab 4 as a whole creates a greater understanding of op-amp circuits by demonstrating the relationship between gain and $V_i$ and $V_o$ as well as demonstrating limitations and behaviors associated with specific types of op-amps through either voltage functions or gain comparisons. After completing this lab, our group will successfully be able to use Op Amps, its circuits, and applications in real-world scenarios.
