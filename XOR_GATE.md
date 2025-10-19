Circuit Description and Functionality

The designed circuit is a CMOS XOR (Exclusive-OR) gate, which produces a high output only when the two inputs are different.
It is implemented using a combination of PMOS and NMOS transistors arranged to realize the logic expression

                                                  𝑌  = 𝐴⊕𝐵
When one input is high and the other is low, the output is driven high. When both inputs are the same (either 0 or 1), the output remains low.
Thus, the circuit performs the XOR logic function used commonly in adders, comparators, and digital arithmetic blocks.

Simulation and Analysis
1. DC Analysis

DC analysis was carried out by sweeping both input voltages to verify the static operation of the XOR gate.
The transfer characteristics show correct logic transitions, with the output switching high only when the inputs differ.
The DC response confirms proper voltage levels, switching threshold, and balanced logic behavior.

2. Transient Analysis

Transient simulation was performed using pulse waveforms for both inputs.
The output waveform shows high output when one input is high and the other is low, and low output when both inputs are equal — confirming accurate XOR functionality.
The propagation delays and switching transitions were observed to be within expected limits, ensuring correct timing performance.


3. Results

The CMOS XOR gate exhibits correct functional behavior, showing high output only for unequal inputs.
The simulation validates full logic swing, low static power, and proper timing response, confirming a reliable transistor-level design.
