### SYNCHRONOUS-UP-COUNTER
# NAME:VINOTH K R
#REG.NO:212224050060


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
![Screenshot 2025-05-06 061919](https://github.com/user-attachments/assets/e7e1e1ca-9fc4-4725-8d51-26b55237281c)


**PROGRAM**
![image](https://github.com/user-attachments/assets/07493e1c-be58-4848-beba-981fa73a4537)




**RTL LOGIC UP COUNTER**
![image](https://github.com/user-attachments/assets/3dd647f3-1280-4f12-90cc-37dec739d66c)


**TIMING DIAGRAM FOR IP COUNTER**
![image](https://github.com/user-attachments/assets/45729301-0822-43d1-b40e-6b86aa4d43e8)



**TRUTH TABLE**

![image](https://github.com/user-attachments/assets/85025b4e-8207-4bba-b87b-cdae394a8943)

**RESULTS**
Hence a 4 bit synchronous up counter is implemented correctly
