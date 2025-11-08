# Two-Stage CMOS Operational Amplifier Layout

The Two-Stage CMOS Operational Amplifier (Op-Amp) is one of the most widely used analog circuits in integrated circuit design.
This project presents the complete analog layout flow, including schematic capture, device placement, routing, and post-layout verification, designed using Cadence Virtuoso and verified with Mentor Calibre.

🧩 Design Overview

The two-stage CMOS Op-Amp consists of:

Differential Input Stage (M1–M4) – Converts the input voltage difference into a current.

Current Mirror Load (M5–M6) – Provides active loading and biasing.

Gain Stage (M7–M8) – Amplifies the voltage swing and drives the output.

Biasing Circuit – Establishes stable operating points for all transistors.

🧠 Circuit Principle

The amplifier converts a differential input voltage into a single-ended output with high gain.
Its two-stage structure achieves:

High open-loop gain (AOL)

Large output voltage swing

Good common-mode rejection ratio (CMRR)

High slew rate and output impedance
Av​=gm1​×(ro2​∣∣ro4​)×gm6​×ro6​	​

# Layout Design Flow
1️⃣ Schematic Design

Circuit topology created in Cadence Virtuoso Schematic Editor.

DC and transient simulations performed using ADE (Analog Design Environment).

2️⃣ Floorplanning

Devices arranged based on signal flow and symmetry considerations.

Differential input pair placed close together for common-centroid matching.

3️⃣ Placement & Matching

Matched devices (M1–M2, M3–M4, and M5–M6) use Common-Centroid and Interdigitation techniques to minimize offset and process variation effects.

Dummy transistors used at edges to ensure uniform boundary conditions.

4️⃣ Routing

Symmetrical metal routing ensures balanced parasitic capacitance.

Poly and metal layers aligned for minimal resistance variation.

5️⃣ Verification

Design Rule Check (DRC) — No violations.

Layout Versus Schematic (LVS) — Matched successfully.

Parasitic Extraction (PEX) — Used to verify post-layout performance.

🧰 Tools Used
Tool	Purpose
Cadence Virtuoso	Schematic design, layout, and simulation
Mentor Calibre	DRC and LVS verification
Linux Environment	For tool integration and project setup
🧩 Matching Techniques Applied

Common Centroid Layout: Minimizes gradient-induced mismatch.

Interdigitation: Alternates matched device fingers for uniform stress and process conditions.

Dummy Transistors: Reduces edge effects for better device uniformity.

📊 Results
Parameter	Description
DRC	No rule violations
LVS	Schematic and layout matched
Symmetry	Maintained for differential pair
Performance	Verified post-layout for DC gain, slew rate, and CMRR
🎯 Learning Outcomes

✅ Understanding of differential pair biasing and mirroring
✅ Implementation of matching-aware layout techniques
✅ Hierarchical analog layout flow
✅ Verification using Calibre DRC & LVS
✅ Hands-on experience in precision analog design

📘 Project Documentation

📄 View Full Op-Amp Layout Portfolio PDF
