# Lab Report 4 - Go Big: Operational Amplifiers
Eli Barrow & Isaac Stevens

Feb. 8, 2024

## Summary of Lab ##



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

**Response:** The LM741 op-amps are symmetric and the positive voltage performance does equal the negative voltage performance for the first circuit until below -12V or above 12V which causes the $V_i$ begins to not equal $V_o$.

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

Note: Since we were running low on time in the lab we did not connect the function generator to find out an record what the frequency limit was for the 741 op amp.     'THIS MAY NEED TO HAVE MORE EXPLANATION BUT I AM NOT SURE' 


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
