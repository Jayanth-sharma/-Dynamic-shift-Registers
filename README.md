# Design of 1bit-Dynamic-shift-Registers in 32nm CMOS technology
# Content
[Abstract](https://github.com/Jayanth-sharma/-Dynamic-shift-Registers#abstract)
[Circuit details](https://github.com/Jayanth-sharma/-Dynamic-shift-Registers#circuit-details)
[Circuit diagram](https://github.com/Jayanth-sharma/-Dynamic-shift-Registers#circuit-details)
[Generated waveforms from simulations](https://github.com/Jayanth-sharma/-Dynamic-shift-Registers#generator-waveform-from-simulation)
[Conclusion](https://github.com/Jayanth-sharma/-Dynamic-shift-Registers#conclusion)


# Abstract
The scope of this project  is to design a dynamic Shift register. Which is a low power consumption and lower area compared to a conventional as well ratioed counterpart.we examine the basic dynamic operations of 2-phase clock shift registers.Dynamic shift registers are simpler in terms of fabrication and have high package density due to their smaller size. However it is to be noted that their advantage of less power consumption is cursed by the fact that the power consumed increases with the increase in frequency. 

# Reference Circuit Diagram
  ![reference_circuit](https://user-images.githubusercontent.com/53760504/156198052-de9f242b-c43e-4dfb-8b4e-60544b7c3d5b.jpg)
#  Circuit Details
Dynamic shift register have several advantages over the Static shift register in terms of higher performance,transistor density, Reduction in circuit delay and silicon area. In each stage, the input pass transistor and the load transistor are driven by the same clock phase.<br />
•Φ1 active.<br />
–Vin transfer to Cin⇒1st inverter is active ⇒Vout1 attains its valid logic level<br />
•Φ2 active <br />
–2nd pass transistor on ⇒the logic level is transferred onto the next stage.<br />
Considering two cases.<br />
–Case 1, <br />
If Cout1 high at the end of the active<br />
Φ1 phase,  <br />
By mean of Cin1 low input ⇒nMOS driver off ⇒Vout1=VDD-VTn.<br />
Φ2 active<br />
The voltage level is transfer to Cin2 via charge sharing over the pass transistor<br />
Cout/Cin↑to correctly transfer a logic-high level<br />
•Considering Case 2<br />
•If Vout1 is logic-low at the end of the active Φ1 phase<br />
Cin1 high, nMOS driver on⇒Vout1=0V<br />
•As Φ2 active<br />
–Transfer by pass transistor<br />
•Ratiolessdynamic logic<br />
–VOL=0, independent of driver-to-load ratio<br />

# Circuit diagram 

![Circuit_diagram](https://user-images.githubusercontent.com/53760504/156196717-b750c060-27c0-41a2-ad17-febf66137ce1.jpg)
![test_bench](https://user-images.githubusercontent.com/53760504/156196870-4c069a84-e2fb-460e-aefd-7e951560e1ac.jpg)

#  Generator waveform from Simulation
![1_bit_shift](https://user-images.githubusercontent.com/53760504/156197016-23d56d55-cd0e-41ec-a480-8c68781aeeae.jpg)

#  Conclusion 
The transient Analysis is done and Understood the flow in Designing of Analog circuit and Analysis.With Synopsys Custom complier tool
# Thanks to 
[VSD](https://www.vlsisystemdesign.com/basic_courses/),[IITH](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/) and [Synopsys](https://www.synopsys.com/) for Organising the hackthon.<br />
[Kunal(VSD founder)](https://github.com/kunalg123),Chinmaya Panda and everyone in the hackthon forum for the help.Had a great time.<br />
[Sameer S Durgoji](https://github.com/SameerSDurgoji) for the Custom complier walkthrough.

# Reference
Razavi, Behzad. 2001. Design of analog CMOS integrated circuits.Boston, MA: McGraw-Hill.<br />
"A design method of nMOS dynamic shift registers for small liquid crystal displays"Shuji Tsukiyama; Shinji Higa
