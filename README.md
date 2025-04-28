### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

Step 1: Write the Truth Table

Step 2: Derive Boolean Expressions

Step 3: Write the Module Declaration

Step 4: Implement Dataflow Assignments

Step 5: Verify by Simulation (Optional but Recommended)

**PROGRAM**

 
Developed by: VENKATA MOHAN N RegisterNumber:212224230298

    Module enc(A0,A1,A2,D0,D1,D2,D3,D4,D5,D6,D7);
    input A0,A1,A2;
    output D0,D1,D2,D3,D4,D5,D6,D7;
    assign A0= ( D4 | D5 | D6 | D7);
    assign A1= ( D2 | D3 | D6 | D7);
    assign A2= ( D1 | D3 | D5 | D7);
    endmodule

    
**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![image](https://github.com/user-attachments/assets/a1764fde-4c26-4f8b-8d96-5e29aee3be4f)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![image](https://github.com/user-attachments/assets/b9387d7c-b3a1-47b5-b23e-5725c8a159c8)


**RESULTS**
Thus the Encoder 8 To 3 in Dataflow Modelling using verilog are verified and the logic diagrams are designed and the truth table is verified.






