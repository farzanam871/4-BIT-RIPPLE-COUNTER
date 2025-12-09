# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**
module asynchronouscounter
input clk,
clock input
);
input reset,
output [3:0]
asynchronous
4-bit output
reset
// Internal flip-flop register
reg [3:e] qreg;
// output assignment
assign q = q_reg;
// FFe toggles with external clock
always e(posedge clk or posedge reset)
if(reset)
begin
end
else
q_reg[e] <= 1'be;
qreg[e] <= q_reg[e];
// FF1 toggles with Qo
always @(posedge q reg[e] or posedge reset) begin
if (reset)
end
else
q_reg[1] <= 1'be;
q_reg[1] <= q_reg[1];
// FF2 toggles with 01
always @(posedge q reg[1] or posedge reset) begin
if(reset)
end
else
q_reg[2] <= 1'be;
q_reg[2] <= q_reg[2];
// FF3 toggles with Q2
always @(posedge q reg[2] or posedge reset) begin
if(reset)
end
else
q_reg[3]<= 1'be;
q_reg[3] <= ~q_reg[3];
endmodule

 Developed by:Farzana Mubarak RegisterNumber:25013772


**RTL LOGIC FOR 4 Bit Ripple Counter**  

<img width="631" height="774" alt="Screenshot 2025-12-09 215344" src="https://github.com/user-attachments/assets/4460ef9a-552d-4407-b822-eca9024e2ee9" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="768" height="404" alt="Screenshot 2025-12-09 215402" src="https://github.com/user-attachments/assets/663049b5-aff4-4e75-8025-18376f340f6f" />

**RESULTS**
Thus 4 BIT-RIPPLE COUNTER is verified successfully
