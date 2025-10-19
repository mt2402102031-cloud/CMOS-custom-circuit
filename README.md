# CMOS-custom-circuit
Design of Custom ALU using CMOS Cells (180 nm Technology)
🧩 Project Overview

This project focuses on the transistor-level design and simulation of a 4-function Arithmetic Logic Unit (ALU) using CMOS logic cells at the 180 nm technology node.
All gates and functional blocks were designed, simulated, and analyzed in Cadence Virtuoso using custom transistor-level schematics.


⚙️ Objectives

Design fundamental CMOS logic gates with minimum transistor count.
Characterize delay, power, and noise margins for each logic cell.
Develop higher-level building blocks like adder and multiplexers using custom cells.
Integrate all modules into a fully functional 4-operation ALU.

🧠 Technology and Tools

Technology Node: 180 nm
Supply Voltage (VDD): 1.2 V
EDA Tool: Cadence Virtuoso (Schematic & Simulation)
Simulation Type: Transient, DC, and Parametric Analysis


🔩 Design Implementation
1. CMOS Logic Gates

Designed using standard CMOS logic principles:

   Gate	     Transistor_Count	   Simulation_Performed	     Parameters_Extracted
   NOT	           2	               Transient	           Delay, Power, Noise Margin
   NAND	           4	               Transient	           Delay, Power, Noise Margin
   NOR	           4	               Transient	           Delay, Power, Noise Margin
   XOR	           10	               Transient	           Delay, Power, Noise Margin
   XNOR	           10	               Transient	           Delay, Power, Noise Margin  

Each gate was verified using transient simulation, and propagation delays were calculated between each input–output transition.

2. Full Adder Design

Implemented a 32-transistor full adder using custom XOR, AND, and OR gates.
Verified functionality for all input combinations using transient analysis.
Measured Power: ~4.62 µW at 1.2 V supply.

3. Multiplexer Design

Designed a 2×1 MUX using 14 transistors from custom logic gates.
Extended to 4×1 MUX using a hierarchical approach (three 2×1 MUX).

Measured Power:
               2×1 MUX → 1.52 µW
               4×1 MUX → 3.56 µW

4. ALU Integration

Developed a 4-function ALU with following operations:
00 → ADD
01 → SUBTRACT
10 → OR
11 → AND

Implemented function selection using a 4×1 MUX as control logic.
Measured Total Power: 11.88 µW at 1.2 V (for 15 ns operation period).

📊 Analysis & Observations

Propagation Delay: Dependent on logic complexity and transistor sizing.

Noise Margin: Verified from inverter VTC; with min W/L ratios.

Power Optimization: Achieved through minimal transistor count and controlled switching activity.

Functional Verification: Successful logical operation across all test vectors for ALU modes.

🧾 Key Learnings

Hands-on understanding of transistor-level CMOS design and simulation.
Experience in power–delay trade-off, noise margin analysis, and hierarchical cell design.
Practical exposure to custom cell integration and circuit-level debugging in Cadence Virtuoso.

🧰 Future Scope

Extend ALU operations (e.g., XOR, XNOR, NAND, NOR).
Perform layout design, DRC/LVS checks, and post-layout simulation using extracted parasitics.
Integrate into a custom datapath for small processor design.
