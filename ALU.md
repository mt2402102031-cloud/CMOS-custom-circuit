Design and Implementation of CMOS-Based ALU
1. Circuit Description

The designed Arithmetic Logic Unit (ALU) performs basic arithmetic and logical operations at the transistor level using CMOS logic.
The ALU structure is modular, consisting of fundamental building blocks such as the Adder circuit, 2:1 Multiplexer, and 4:1 Multiplexer.
These subcircuits are integrated to implement functions like addition, logical operations, and selection of outputs based on control signals.


<img width="634" height="522" alt="ALU" src="https://github.com/user-attachments/assets/7f5b1d05-633d-47ae-8d71-2225c8ab84e4" />

2. Functional Blocks

Adder Circuit:
The adder is designed using CMOS logic to perform binary addition of two input bits.
It generates Sum and Carry outputs which form the arithmetic part of the ALU.
The implementation ensures full voltage swing and minimum static power consumption.

<img width="648" height="396" alt="ADDER" src="https://github.com/user-attachments/assets/93239928-617a-463d-bb5a-94f21323d390" />

2:1 Multiplexer:
The 2:1 MUX selects between two input signals based on a single select line.
It is used in the ALU for controlling data paths and enabling operation selection.


<img width="687" height="356" alt="2X1MUX" src="https://github.com/user-attachments/assets/3e12339e-be8f-489f-b8b8-9ce1b58d279f" />

4:1 Multiplexer:
The 4:1 MUX is used at the output stage of the ALU to select one of four possible operation results based on two control inputs.
It ensures efficient operation decoding and compact routing.


<img width="641" height="470" alt="4X1MUX" src="https://github.com/user-attachments/assets/f6ffc014-1931-4369-a2d7-79c4779eb9f4" />


3. Transient Simulation and Analysis

Transient analysis was carried out to verify the functional behavior of the complete ALU.
Different input combinations and control signals were applied to check all arithmetic and logic operations.
The output waveform demonstrates correct switching between operations, confirming that the ALU performs as expected.

<img width="1001" height="638" alt="TR1" src="https://github.com/user-attachments/assets/2c546609-af9a-4517-ab7c-e7f2316aea40" />

4. Results and Discussion

The designed CMOS-based ALU successfully integrates arithmetic and logic modules using basic transistor-level blocks.
The transient simulation confirms correct operation for all tested logic functions, and the power analysis indicates low-power performance.
