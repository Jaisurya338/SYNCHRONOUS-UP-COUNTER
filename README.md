### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:
![WhatsApp Image 2025-10-16 at 16 01 37_6e19adcb](https://github.com/user-attachments/assets/3e411fb2-ef84-41f8-8002-f833fb0651ec)


Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**
<img width="1826" height="980" alt="Screenshot 2025-10-16 180036" src="https://github.com/user-attachments/assets/9a101f3c-53ae-4c72-9207-9cf0f2394136" />

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by:Ramesh Jaisurya

 RegisterNumber:2500580
*/

**RTL LOGIC UP COUNTER**
![WhatsApp Image 2025-10-16 at 16 01 31_c6f8a8a5](https://github.com/user-attachments/assets/6da4fbfe-5c2a-46d9-87f6-4533aeb040c4)

**TIMING DIAGRAM FOR IP COUNTER**

**TRUTH TABLE**

**RESULTS**
thus,the given logic is studied and verified successfully
