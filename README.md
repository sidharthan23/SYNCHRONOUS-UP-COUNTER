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
**PROGRAM**

**Program for flipflops and verify its truth table in quartus using Verilog programming.**

**Developed by: Sidharthan V**
**RegisterNumber:212223050049**
![330487250-11c16ec7-4de3-4675-a190-60cebff36125](https://github.com/monish1545/SYNCHRONOUS-UP-COUNTER/assets/166646660/3b0c6748-6d24-42a8-a991-5ce6807f43b9)

**RTL LOGIC UP COUNTER**
![330487316-a2623159-bba6-473d-a6c2-a05fd32d017d](https://github.com/monish1545/SYNCHRONOUS-UP-COUNTER/assets/166646660/a7103df8-1475-4578-8859-f23be45c2b32)

**TIMING DIAGRAM FOR IP COUNTER**
![330487515-54ada763-d19c-441d-9ecb-18a948a256f8](https://github.com/monish1545/SYNCHRONOUS-UP-COUNTER/assets/166646660/2d407675-7b61-46f6-aa9e-8ed22d23f7a3)

**TRUTH TABLE**
![330487597-dfaccd3f-54ee-41ba-b91a-d9034cc9c520](https://github.com/monish1545/SYNCHRONOUS-UP-COUNTER/assets/166646660/9c0bb069-e03a-4aba-b1a9-19f440c4491c)

**RESULTS**
Thus the program executed successfully.
