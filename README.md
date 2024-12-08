EXP 3:HALF ADDER AND HALF SUBTRACTOR

NAME: AANANDHA KANNAN.S

REF NO: 24900501

AIM

TO DESIGN HALF ADDER AND HALF SUBTRACTOR FOR CIRCUIT AND VEROFY ITS TRUTH TABLE IN QUARTUS USING VENILOG PROGRAMMING

Equipments Required:

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

HALF ADDER AND HALF SUBTRACTOR

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)


 

Figure -02 HALF Subtractor

**Truthtable**
1) HALF ADDER
![Screenshot 2024-12-08 222024](https://github.com/user-attachments/assets/54a34128-1b1a-4086-ae4c-2662587b16d2)
2) HALF SUBTRACTOR
![Screenshot 2024-12-08 222043](https://github.com/user-attachments/assets/8171ffe1-5fa9-45e0-9494-be3109d1ee66)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.



**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
 1) HALF ADDER
module halfadd(a,b,sum,count);

input a,b;

output sum,count;

xor (sum,a,b);

and (cout,a,b);

endmodule

2)HALF SUBTRACTOR
module halfsub(a,b,diff,borr);

input a,b;

output diff,borr;

wire w1;

xor g1(diff,a,b);

not g2(w1,a);

and g3(borr,w1,b);

endmodule 


 


**RTL Schematic**
1) HALF ADDER

![HALF ADDER](https://github.com/user-attachments/assets/643b02aa-501d-434b-af53-4e3893c384f8)

 2)HALF SUBTRACTOR
 
 ![Screenshot 2024-12-08 223541](https://github.com/user-attachments/assets/1ce4e924-721d-4197-8698-fa31fbc54486)



 

**Output/TIMING Waveform**
1) HALF ADDER

![HA WF](https://github.com/user-attachments/assets/464b025b-6d30-4531-84bd-695eeb28205b)



2)HALF SUBTRACTOR

![HS WF](https://github.com/user-attachments/assets/aeda0477-ad39-484c-9273-b25c6661a16a)



**Result:**
THUS THE HALF ADDER AND HALF SUBTRACTOR CIRCUITS ARE DESIGNED AND TRUTH TRABLE IS VERIFIED USING QUARTUS SPOFTWARW
