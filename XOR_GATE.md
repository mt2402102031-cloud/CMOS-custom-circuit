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

<img width="1908" height="816" alt="vtcA=0" src="https://github.com/user-attachments/assets/5362371e-9238-4453-8b75-26ce9796b141" />

<img width="1898" height="806" alt="vtcA=1 2" src="https://github.com/user-attachments/assets/d9af8112-ce16-414c-9153-32bce5632813" />

<img width="1888" height="753" alt="vtcB=0" src="https://github.com/user-attachments/assets/2aae7fcd-a066-4657-baaa-4bdf7a0e956c" />

<img width="988" height="636" alt="vtcB=1 2" src="https://github.com/user-attachments/assets/90af5090-f9b5-4da8-bca0-f91ca179ca4d" />


2. Transient Analysis

Transient simulation was performed using pulse waveforms for both inputs.
The output waveform shows high output when one input is high and the other is low, and low output when both inputs are equal — confirming accurate XOR functionality.
The propagation delays and switching transitions were observed to be within expected limits, ensuring correct timing performance.


<img width="1901" height="831" alt="XorTAtY" src="https://github.com/user-attachments/assets/74c59f92-6845-4368-8d4f-8d20f2d4cbb4" />

<img width="1891" height="828" alt="XorTBtY" src="https://github.com/user-attachments/assets/ad454f40-43a7-43b2-b843-46c5631de77d" />

3. Glitches


<img width="1000" height="636" alt="AB(11_GLITCH)" src="https://github.com/user-attachments/assets/df7de727-7cfe-4a1f-91e0-8bb9d65e6b0d" />

<img width="994" height="641" alt="glitch2" src="https://github.com/user-attachments/assets/ca538e3b-542b-4ebf-9dd3-d767c7c2368c" />

<img width="998" height="640" alt="glitches3" src="https://github.com/user-attachments/assets/89a1b795-23d4-451a-a68d-f624643359da" />

<img width="995" height="669" alt="glitch4" src="https://github.com/user-attachments/assets/e0686972-8e9c-4376-bf7e-543cb39ce356" />


4. Results

The CMOS XOR gate exhibits correct functional behavior, showing high output only for unequal inputs.
The simulation validates full logic swing, low static power, and proper timing response, confirming a reliable transistor-level design.
