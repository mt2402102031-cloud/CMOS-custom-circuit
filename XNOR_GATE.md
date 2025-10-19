Circuit Description and Functionality

The designed circuit is a CMOS XNOR (Exclusive-NOR) gate, which produces a high output when both inputs are equal.
It is realized using complementary PMOS and NMOS networks that implement the logic expression

                                      Y = ~(A⊕B)​
When both inputs are low or both are high, the output goes high; otherwise, the output remains low.
This gate is widely used in comparators, equivalence checkers, and digital arithmetic circuits.

<img width="522" height="453" alt="xnorckt" src="https://github.com/user-attachments/assets/a8ab189c-e081-47d0-a041-4f45264b8828" />


1. DC Analysis

DC analysis was performed to verify the static operation of the XNOR gate.
By sweeping the input voltages, the output behavior was observed to ensure correct logic transitions.
The DC transfer characteristics confirm that the output remains high when both inputs are the same, demonstrating proper static operation and balanced switching thresholds.


<img width="1839" height="764" alt="DC1" src="https://github.com/user-attachments/assets/82e3a498-cba7-4a5f-a172-0d3663d7365f" />

<img width="1912" height="817" alt="DC2" src="https://github.com/user-attachments/assets/b924acc6-c20d-42da-943e-2f659b6b2bab" />

<img width="1907" height="812" alt="DC3" src="https://github.com/user-attachments/assets/cd1d2241-fd62-49a4-b86a-b8a858400d8f" />

<img width="1911" height="813" alt="DC4" src="https://github.com/user-attachments/assets/887082ea-d71a-4d50-85f5-32e5d1b9aa77" />


2. Transient Analysis

Transient simulation was carried out by applying pulse inputs to both terminals.
The output waveform shows high voltage when both inputs are equal and low voltage when they differ, confirming correct XNOR functionality.
Propagation delays and signal transitions were measured and found consistent with expected CMOS behavior.

<img width="1911" height="815" alt="TR1" src="https://github.com/user-attachments/assets/c0a2c1d9-e87c-400c-88fb-7a9353920f90" />

<img width="1917" height="809" alt="TR2" src="https://github.com/user-attachments/assets/af2b2953-1177-42dc-893f-7354d548e8da" />

<img width="1909" height="812" alt="TR3" src="https://github.com/user-attachments/assets/e8314a5d-33ef-4b3c-8ebd-3a9fb028229c" />

<img width="1915" height="807" alt="TR4" src="https://github.com/user-attachments/assets/0db322e4-8a62-4e1f-b8cf-a1379ab6f3b4" />

<img width="1916" height="816" alt="TR5" src="https://github.com/user-attachments/assets/3200f4ac-8b9e-49c5-be98-e9b4d30c29f0" />

<img width="1918" height="820" alt="TR6" src="https://github.com/user-attachments/assets/5e6d7ac3-617f-4fb9-88b5-10fae0ed764e" />

3. Results

The CMOS XNOR gate exhibits proper logic operation with high output for equal inputs and low output for unequal inputs.
The circuit provides full voltage swing, low static power, and reliable dynamic response, verifying successful transistor-level implementation.
