
# Digital layouts
Standard cells are the fundamental building blocks of digital VLSI design.
Each cell implements a specific logic function (e.g., inverter, NAND, XOR, MUX, D-Latch) and is optimized for area, performance, and power.
These cells are designed with uniform height and routing tracks, enabling automated place-and-route integration in larger digital systems.
Standard cells are pre-characterized logic gates and sequential elements used to implement complex digital circuits efficiently.
Each cell is designed at the transistor level and verified for:

Electrical correctness — ensuring functionality across process, voltage, and temperature (PVT) corners

Physical correctness — adhering to design rules (DRC) and layout-versus-schematic (LVS) compliance

🧱 Key Characteristics

Fixed Height, Variable Width: Allows consistent power/ground rail alignment and easy tiling during place-and-route.

Power and Ground Rails: Run horizontally at the top and bottom for uniform connectivity.

Routing Tracks: Provide predictable metal layers for interconnect routing.

Library Compatibility: Cells follow the same design rules and track pitch, making them interchangeable within the same technology node.

🧠 Design Process

Transistor Sizing – Optimize width/length for drive strength and delay.

Layout Design – Place PMOS and NMOS transistors in rows, ensuring symmetry and minimal diffusion breaks.

DRC & LVS Verification – Validate that layout meets foundry rules and matches the schematic.

Characterization – Extract timing, power, and functional models for synthesis and P&R tools.

🧰 Cells Designed in this Portfolio
Cell	Function	Description
INV	Inverter	Basic NOT gate, inverts input logic.
NAND	NAND Gate	Performs AND followed by inversion; universal logic gate.
XOR	Exclusive OR	Outputs HIGH when inputs differ.
MUX (2:1)	Multiplexer	Selects one input based on control signal.
D-Latch	Data Latch	Level-sensitive storage element for sequential circuits.
🧩 Applications

1.ASIC and SoC Digital Core Libraries

2.Arithmetic Logic Units (ALU)

3.Memory and Control Logic Blocks

4.Standard Cell Libraries for Physical Design Flow
