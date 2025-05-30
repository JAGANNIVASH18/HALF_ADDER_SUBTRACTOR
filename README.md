# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/user-attachments/assets/33a93bd6-79cf-4f4d-9ee3-dbe12c560cb7)


Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

![image](https://github.com/user-attachments/assets/ea314292-bf27-4db7-89ae-2ad3f83e88e4)


Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
Developed by: JAGANNIVASH U M
Reg no:. 212224240059
```
```
i)HALF ADDER
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
```
```
ii)HALF SUBTRACTOR
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```
**RTL Schematic**
![image](https://github.com/user-attachments/assets/43a3c60b-4290-4c35-bfbf-d5252c004420)
![image](https://github.com/user-attachments/assets/11494114-efb6-4d01-b28f-a4eface21633)


**Output/TIMING Waveform**
![image](https://github.com/user-attachments/assets/d7d7ff78-903b-4173-9580-457a9118b8cd)
![image](https://github.com/user-attachments/assets/92c4dbb6-4d97-43ed-96a0-4b914a910c6a)


**Result:**
Designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming hence the above the output was verified
