# Design of Common-Source Stage with Resistive Load
The design of Common-Source Stage with Resistive Load is found in this report. The design was developed using the $g_m/I_d$ method, which is organized in the spreadsheet. The simulation results can be viewed in the images below.

## Testbench
![image](https://github.com/user-attachments/assets/d4d90ffc-6320-4999-a0b5-d5f854a6c7ee)

## Schematic
![image](https://github.com/user-attachments/assets/6609504b-7315-4283-a1cf-bfb843cf4ff3)

## Design Variables
![image](https://github.com/user-attachments/assets/5407e4ef-3661-41ca-ba50-8a1bdb347532)

## Simulation Results
When $V_{in}$ is high, $V_{out}$ is low, $M_1$ is in the triode region, and $g_m$ assumes a small value. As $V_{in}$ falls and $V_{out}$ and $g_m$ rise, $M_1$ enters saturation when $V_{in} - V_{out} = V_{TH}$ and $g_m$ reaches its maximum. As $V_{in}$ falls further, so do $I_D$ and $g_m$. When $V_{in}$ is low, $g_m$ reaches zero.

![image](https://github.com/user-attachments/assets/7d0e354d-1690-4295-82b2-6177232ec4ec)

For large values of $R_D$, the effect of channel-lenght modulation in $M_1$ becomes significant. To maximize the voltage gain, we must mazimize (small-signal) the load impedance. Why can we not replace the load with an open circuit because the circuit still needs a path from $V_{DD}$ to ground for the bias current of $M_1$. 

## Conclusion
![image](https://github.com/user-attachments/assets/7eea9f0f-090f-4513-9945-5365f294c28a)

## References
[1] RAZAVI, B. Design of analog CMOS integrated circuits. Tsinghua University Press Co., Ltd., 2005

[2] POSSANI, T., et al. "Application of gm/id methodology for analog design using nanometer-scale devices." XXVIII—South symposium of microelectronics—SIM. 2013.

[3] Electronic Echoes. (Feb 10, 2024). Design of a CMOS Common Source Amplifier using Gm/Id Methodology in Cadence Virtuoso. [Video]. YouTube. https://www.youtube.com/watch?v=rE4TcO9IqR8&t=1s.

[4] Mastering Microelectronics. (Dec 17, 2020). The gm/ID Design Methodology Demystified (English). [Video]. YouTube. https://www.youtube.com/watch?v=dzz4z3ijVts.

[5] TIWARI, A. Design of MOS Amplifiers Using gm/ID Methodology. [Slides]. https://designers-guide.org/forum/Attachments/Gm_BY_ID_Methodology.pdf.
