# Power-Divider-ADS
W-band Power Divider
Power dividers and directional couplers are passive microwave components used to split or combine RF power. In power division, one input signal is divided into two or more outputs, while in power combining, multiple inputs are merged into one output. These devices can have three or more ports and are often designed to be lossless.

Three-port devices (e.g., T-junctions) act as power dividers.

Four-port devices (e.g., directional couplers, hybrids) can split or combine signals with controlled phase and amplitude.
Power dividers typically provide equal, in-phase outputs (3 dB split), though unequal splits are possible. Directional couplers allow arbitrary power division, while hybrid junctions provide equal power division with a 90° or 180° phase difference between outputs.

# Power-Divider Simulation using ADS
Here, a power divider operating in W-band was developed
S21 / S31 ≈ −3.3 to −3.8 dB across 75–110 GHz → close to expected. This indicates the divider is splitting power roughly equally with modest excess loss (reasonable).

S11 / S22 / S33 vary from about −18 to −10 dB (getting worse at high freq) → matching is acceptable at lower end but degrades; not as good as ideal.

S32 (isolation) moves from about −20 dB at 75 GHz to ≈ −6 dB at 110 GHz → isolation becomes poor at higher frequencies.

![3D Model- 4 membranes](https://github.com/samueloladosu37/Power-Divider-ADS/blob/main/Capture%20d'%C3%A9cran%202025-10-15%20154632.png)

![3D Model- 4 membranes](https://github.com/samueloladosu37/PMUT-FEM-Simulation-using-COMSOL/blob/main/3D%20Model%201.png)

# Does this behave like a Wilkinson power divider?

- **Insertion loss (S21, S31):** ~−3.3 to −3.8 dB → close to the expected −3.01 dB for an equal split (small excess loss present).
- **Return loss (S11, S22, S33):** ~−18 to −10 dB → acceptable near low end but degrades at higher frequencies.
- **Isolation (S32/S23):** degrades from ~−20 dB at 75 GHz to ~−6 dB at 110 GHz → poor isolation at the high end.

**Conclusion:** The device performs like a Wilkinson near its design frequency (reasonable split and modest loss), but matching and isolation degrade across the plotted 75–110 GHz band. 
