Circuit Description and Functionality

The designed circuit is a CMOS NAND gate, implemented using two PMOS transistors in parallel and two NMOS transistors in series.
When both inputs are high (logic ‘1’), the NMOS network conducts and the output is pulled low (logic ‘0’).
For all other input combinations, at least one PMOS transistor remains ON, pulling the output high (logic ‘1’).
Thus, the circuit performs the NAND logic operation, where the output is low only when all inputs are high.
<img width="489" height="521" alt="ckt" src="https://github.com/user-attachments/assets/85e3e563-35b2-47a6-b2aa-0ef8ffe1dd42" />

Simulation and Analysis
1. DC Analysis

DC analysis was carried out by sweeping the input voltages to verify the static behavior of the NAND gate.
The transfer characteristics confirm correct logic levels and smooth switching transitions between 0 V and 1.2V.
From the DC curves, the gate shows proper noise margins and threshold behavior, ensuring reliable logic operation.
<img width="1914" height="814" alt="DC1" src="https://github.com/user-attachments/assets/4b995070-f2ec-48b7-8fb4-bca4148816c8" />
<img width="1920" height="816" alt="DC2" src="https://github.com/user-attachments/assets/e22631c5-8f77-4c0d-bc34-4ee0b6734850" />

2. Transient Analysis

Transient simulation was performed using pulse inputs to check the dynamic response of the NAND gate.
The output waveform shows that the output stays high for all input combinations except when both inputs are high — matching ideal NAND logic behavior.
The delay, rise, and fall times observed are within expected limits for the given transistor sizes.
<img width="1909" height="809" alt="Tr1" src="https://github.com/user-attachments/assets/412328d6-a33e-4674-ae95-e3a044d58f71" />
<img width="1919" height="811" alt="Tr2" src="https://github.com/user-attachments/assets/e7a09317-0017-4a3e-bc5d-8cc696b05213" />
<img width="1915" height="809" alt="Tr3" src="https://github.com/user-attachments/assets/3464f79b-47c6-429b-aaad-acfc64852973" />
<img width="1920" height="814" alt="Tr4" src="https://github.com/user-attachments/assets/2c3b3288-6989-4469-9389-19c0d976168f" />

3. Glitches

<img width="1889" height="770" alt="glich1" src="https://github.com/user-attachments/assets/570d4543-93db-43e1-9ae3-d1c29b4c5bde" />

4. Results

Both DC and transient results confirm the correct operation of the CMOS NAND gate.
The circuit provides full logic swing, low static power, and balanced delay characteristics, verifying proper functionality at the transistor level.






