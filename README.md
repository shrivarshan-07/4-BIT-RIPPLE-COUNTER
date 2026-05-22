# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by: Shrivarshan 

 
 RegisterNumber: 212225240146

*/

```
module EXP6(
    input clk,
    input reset,
    output reg [3:0] q
);

always @(posedge clk or posedge reset)
begin
    if (reset)
        q <= 4'b0000;
    else
        q <= q + 1;
end

endmodule
```

**RTL LOGIC FOR 4 Bit Ripple Counter**


<img width="481" height="177" alt="Screenshot 2026-05-21 191140" src="https://github.com/user-attachments/assets/b20ce778-bda3-4862-a615-16e91ef48e4a" />


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1918" height="298" alt="Screenshot 2026-05-21 191325" src="https://github.com/user-attachments/assets/936c3d4c-5649-43b4-a00a-deaca29f59e8" />


**RESULTS**
Thus the program 4 Bit Ripple Counter is verified successfully.
