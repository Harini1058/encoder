# encoder
# AIM:

To implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

# SOFTWARE REQUIRED:
Quartus prime

# THEORY

# Encoder 8 To 3

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

<img width="385" height="318" alt="Screenshot 2025-12-05 221334" src="https://github.com/user-attachments/assets/79d0874d-38f5-4e51-a232-296456286f14" />

Figure 01 Block Diagram of Encoder 8 * 3

# Truth Table

<img width="528" height="409" alt="Screenshot 2025-12-05 221349" src="https://github.com/user-attachments/assets/8dcc615b-7c22-46ae-891c-af4ede28f493" />


The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

<img width="807" height="454" alt="Screenshot 2025-12-05 221455" src="https://github.com/user-attachments/assets/86f3fe87-f319-449d-a2b6-cfe25fd48c19" />


Figure 02 Encoder 8 * 3

# Procedure

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

# PROGRAM

Developed by: Harini G
RegisterNumber: 25015377

module exp5(din,a,b,c);

input [0:7] din;

output a,b,c;

assign a=(din[4]| din[5]| din[6 ]| din[7]);

assign b=(din[2]| din[3]| din[6]| din[7]);

assign c=(din[1]| din[3]| din[5 ]| din[7]);

endmodule

# RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling

<img width="933" height="865" alt="Screenshot 2025-12-05 094357" src="https://github.com/user-attachments/assets/7b806ebc-aa22-42f2-a441-ba7d9c002509" />

# TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling

<img width="1898" height="993" alt="Screenshot 2025-12-05 094955" src="https://github.com/user-attachments/assets/dfc818e7-3b5f-48c9-b820-6db737202477" />

# RESULTS

Implementing Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables executed succesfully.
