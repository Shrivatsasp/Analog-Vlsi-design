# Bit1 Block Digital Design (Mini Project)

The Bit1 Block is a combinational digital circuit that counts the number of logic ‘1’s in its 6-bit input and provides the binary equivalent of that count as output.
It represents a hierarchical design approach, combining smaller verified sub-blocks into a single top-level layout.

🧱 Sub-Blocks Used
Sub-Block	Function
2-Input AND Gate	Basic logical AND function
3-Input AND Gate	Extends logic conjunction for three inputs
OR Gate	Performs logical addition
XOR Gate	Outputs HIGH when inputs differ
Full Adder	Adds three 1-bit inputs (A, B, Cin)
3-Bit Ones Block	Counts the number of ones in 3-bit input

Each sub-block is verified with truth tables and testbench waveforms to ensure functional correctness.

⚙️ Working Principle

The Bit1 Block processes six input bits to compute how many are logic HIGH (1).
It uses combinational adders and logic gates arranged hierarchically to perform bit counting.

Output (M2, M1, M0)
=
Binary representation of total 1’s in input
Output (M2, M1, M0)=Binary representation of total 1’s in input
📈 Performance Analysis
Process	Voltage	Temp	TPLH	TPHL	Current
FF	1.98 V	0 °C	618.87 ps	696.24 ps	1.52 µA
TT	1.8 V	27 °C	849.22 ps	927.60 ps	1.33 µA
SS	1.62 V	100 °C	1.138 fs	1.918 fs	1.21 µA

Total Transistors: 228
Total Layout Area: 997.92 µm²

🧩 Floorplan and Layout

Designed and routed hierarchically using Cadence Virtuoso.

Power mesh integrated for stable distribution.

Each sub-block (Full Adder, 3-Bit Ones, and Bit1 Block) verified DRC & LVS clean using Mentor Calibre.

⚙️ Applications

Digital Signal Processing (DSP)

Arithmetic Logic Units (ALU)

Parity and Error Detection Circuits

🎯 Learning Outcomes

✅ Floorplanning and placement strategy
✅ Hierarchical routing methodology
✅ Power mesh creation
✅ Debugging DRC/LVS errors
✅ Timing path analysis and optimization

⚙️ Challenges Faced

Handling EXOR layout in 13 CPP

Managing routing congestion in Ones_3_Bit block

Longest path delay identification

Ensuring power mesh compatibility during routing

4.Standard Cell Libraries for Physical Design Flow
