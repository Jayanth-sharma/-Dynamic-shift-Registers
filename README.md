# Design of 1bit-Dynamic-shift-Registers in 28nm CMOS technology
# Content
<ul>
<li>Abstract</li>
<li>Circuit details</li>
<li>Circuit diagram </li>
<li>Generated waveforms from simulations</li>
<li>Conclusion</li>
</ul>

# Abstract
The scope of this project  is to design a dynamic Shift register. Which is a low power consumption and lower area compared to a conventional as well ratioed ocounterpart.we examine the basic dynamic operations of 2-phase clock shift registers.Dynamic shift registers are simpler in terms of fabrication and have high package density due to their smaller size. However it is to be noted that their advantage of less power consumption is cursed by the fact that the power consumed increases with the increase in frequency. 

# Reference Circuit Diagram
  ![reference_circuit](https://user-images.githubusercontent.com/53760504/156198052-de9f242b-c43e-4dfb-8b4e-60544b7c3d5b.jpg)
#  Circuit Details
Dynamic shift register have several advantages over the Static shift register in terms of higher performance,transistor density, Reduction in circuit delay and silicon area. In each stage, the input pass transistor and the load transistorare driven by the same clock phase
•Φ1 active
<li>–Vin transfer to Cin⇒1st inverter is active ⇒Vout1 attains its valid logic level</li>
•Φ2 active
–2nd pass transistor on ⇒the logic level is transferred onto the next stage
Considering two cases
–Case 1
If Cout1 high at the end of the active
Φ1 phase
By mean of Cin1 low input ⇒nMOS driver off ⇒Vout1=VDD-VTn
Φ2 active
The voltage level is transfer to Cin2 via charge sharing over the pass transistor
Cout/Cin↑to correctly transfer a logic-high level
•Considering Case 2
•If Vout1 is logic-low at the end of the active Φ1 phase
Cin1 high, nMOS driver on⇒Vout1=0V
•As Φ2 active
–Transfer by pass transistor
•Ratiolessdynamic logic
–VOL=0, independent of driver-to-load ratio
#  Circuit diagram 
![Circuit_diagram](https://user-images.githubusercontent.com/53760504/156196717-b750c060-27c0-41a2-ad17-febf66137ce1.jpg)
![test_bench](https://user-images.githubusercontent.com/53760504/156196870-4c069a84-e2fb-460e-aefd-7e951560e1ac.jpg)

#  Generator waveform from Simulation
![1_bit_shift](https://user-images.githubusercontent.com/53760504/156197016-23d56d55-cd0e-41ec-a480-8c68781aeeae.jpg)
toll
#  Conclusion 
The transient Analysis is done and Uunderstood the flow in Designing of Analog circuit and Analysis.With Synopsys Custom complier tool
