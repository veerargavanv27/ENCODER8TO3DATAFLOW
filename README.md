### ENCODER 8TO3 DATAFLOW Modelling

# AIM:

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

# SOFTWARE REQUIRED:
Quartus prime

# THEORY

# Encoder 8 To 3:

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

# Truth Table:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

# Procedure:

STEP-1 Define Inputs and Outputs

STEP-2 Understand the Encoder Functionality

STEP-3 Design the Functional Table

STEP-4 Write Verilog Code

STEP-5 Verify Verilog Code

STEP-6 Synthesize the Design

STEP-7 Implement in FPGA

STEP-8 Verify Functionality on FPGA


# PROGRAM
Developed by: VEERARAGAVAN V
Register number: 212223230237
``` 
module Exp_05(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule
```

# RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling:
![image](https://github.com/arbasil05/ENCODER8TO3DATAFLOW/assets/144218037/4770a540-e3ff-4db7-9e80-86ae01ccc650)


# TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling:
![image](https://github.com/arbasil05/ENCODER8TO3DATAFLOW/assets/144218037/db92d594-8fcc-4c2c-b694-feca6050ce08)


# RESULTS:
Thus the given experiment is completed successfully




