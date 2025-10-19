Circuit Description and Functionality

The designed circuit is a CMOS NOR gate, implemented using two PMOS transistors in series and two NMOS transistors in parallel.
When both inputs are low (logic ‘0’), the PMOS network conducts and pulls the output high (logic ‘1’).
For any input combination where at least one input is high, the NMOS network conducts, pulling the output low (logic ‘0’).
Hence, the circuit performs the NOR logic operation, where the output is high only when all inputs are low.

Simulation and Analysis
1. DC Analysis

DC analysis was performed to examine the static behavior of the NOR gate.
By sweeping the input voltages, the output voltage variation was observed to confirm the correct logic transitions.
The transfer characteristic shows proper switching between logic levels, validating the expected NOR function and balanced threshold voltage.


<img width="1917" height="817" alt="vtcA=0" src="https://github.com/user-attachments/assets/3d3a9832-5757-42c8-9f3c-2d8e5d47a1ce" />

<img width="1913" height="814" alt="vtc2" src="https://github.com/user-attachments/assets/87867052-830e-4eb0-b7af-94c05e8e0564" />

<img width="1882" height="756" alt="vtc3" src="https://github.com/user-attachments/assets/c3b83c4f-e772-41a3-91e3-e481c7227f7d" />




2. Transient Analysis

Transient simulation was done by applying pulse signals to both inputs.
The output waveform shows high output only when both inputs are low, and low output otherwise — confirming correct NOR logic operation.
The simulated waveforms indicate clean transitions and acceptable propagation delays for the given transistor dimensions.


<img width="1920" height="845" alt="Nor_AtY" src="https://github.com/user-attachments/assets/3f8483a8-993f-418c-a809-0dbc00b3fb42" />

<img width="1903" height="830" alt="Nor_TBtY" src="https://github.com/user-attachments/assets/0ec5d35d-93cd-4e8e-a138-85ca6de8b852" />



3. Results

Simulation results verify that the designed CMOS NOR gate works correctly.
The circuit exhibits full logic swing, low static power dissipation, and stable operation, confirming reliable transistor-level implementation.
