# recruit-vicharak
A simple Class-D amplifier designed in KiCad, using LM393 comparator and BC107 transistors. Demonstrates PWM-based audio amplification with an LC filter. Includes schematic, PCB layout, and BOM. Open-source for learning and experimentation in high-speed digital and analog circuit design.

The design demonstrates the working principle of Class-D amplification:
Input signal → converted into PWM by LM393
Transistor stage (Q1, Q2) → switching output
LC filter → smoothens PWM into analog audio

Circuit Description:
LM393 Comparator: Generates the PWM based on input reference.
Q1 & Q2 (BC107 transistors): Push-pull stage for amplification.
LC Filter (L1, C1): Filters high-frequency switching, leaving amplified audio.
R1 (1kΩ): Load resistor.
Supply Voltage: +15V

Components Used:
LM393 – Comparator
BC107 × 2 – Transistors
Inductor L1
Capacitor 1µF
Resistor 1kΩ

Simulation / Testing:
Mention whether you simulated in KiCad (ngspice) or plan to.
Expected output: PWM switching at transistors, filtered sine/audio at load.

PCB Design Notes:
Mention that PCB is routed in KiCad.
Short gate traces, separate power/signal section, ground plane for stability.

Future Improvements:
Replace BC107 with MOSFETs for higher efficiency.
Add proper gate driver IC.
Use feedback loop for distortion reduction.
