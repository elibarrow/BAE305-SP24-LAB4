# Lab Report 4 - Go Big: Operational Amplifiers
Eli Barrow & Isaac Stevens
Feb. 8, 2024

## Summary of Lab ##



### Lab Objective: Learn to use Op Amps, it's circuits and applications ###  



## Lab Assignment Specific Items ##



## Part 1 - Limits of Op Amps##
We began this lab by constructing the unity gain inverting op amp circuit shown below.

<p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%201.png width=35%>
</p>

We drove the voltage divider with the positive and negative voltage supplies from the DC Power Supply: Global Specialties 1403. We then collected $V_o$ and $V_i$ data by adjusting the potentiometer to change the input voltage. We collected 9 values that range from the negative and positive saturation points. 


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


 After completing the gain analysis for that circuit we then moved on to analyze another circuit, which is shown below.

 <p align="center">
  <img src=https://github.com/elibarrow/BAE305-SP24-LAB4/blob/main/Circuit%202.png width=35%>
</p>

After constructing this circuit we connected the function generator to $V_i$ and used the oscilloscope to plot $V_i$ in channel 1 and $V_o$ in channel 2.



## Part 2 - Op Amps and frequency response ##
