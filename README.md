### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**


**PROGRAM**

Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: MANOJ KUMAR N
RegisterNumber:25015346


**RTL LOGIC UP COUNTER**

**TIMING DIAGRAM FOR IP COUNTER**

**TRUTH TABLE**

**RESULTS**
RTL VIEWER:
<img width="1919" height="1079" alt="RTL VIEWER EX11" src="https://github.com/user-attachments/assets/c968e5cc-a7be-47d4-97e7-6bcf53edcd6a" />
WAVEFORM:
<img width="1919" height="1079" alt="WAVEFORM EX11" src="https://github.com/user-attachments/assets/0694f6f5-17f4-410c-a4f7-01a2197a0bbc" />

