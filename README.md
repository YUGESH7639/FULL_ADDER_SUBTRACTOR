# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

![tt 1](https://github.com/user-attachments/assets/74ddf1d8-a8e4-4b48-a541-ed8b8c77d36f)


![tt2](https://github.com/user-attachments/assets/5be0a712-b664-4230-a407-974f385a17ac)



**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:YUGESH M


RegisterNumber:24900164


i)FULL ADDER



module fa(a,b,cin,sum,carry);


input a,b,cin;


output sum,carry;


assign sum=( (a ^ b)^c);


assign carry= ( (a & b)| ( cin &(a ^ b ));


endmodule






ii)FULL SUBTRACTOR



module fs(a,b,difference,borrow);


input a,b,bin;


output difference,borrow;


assign difference= ( (a ^ b)^bin);


assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b )));


endmodule




*/

**RTL Schematic**

![exp 4,1](https://github.com/user-attachments/assets/b49d7417-d4b2-46c1-a927-86e526e65d6a)



![exp 4,2](https://github.com/user-attachments/assets/5f41e2bd-8846-4e86-8af4-0a9211682988)


**Output Timing Waveform**

![exp t 4,1](https://github.com/user-attachments/assets/fa387592-21b2-4551-9c69-7f9870a44a9d)


![exp 4 t,2](https://github.com/user-attachments/assets/b6e73ae7-6c7a-4019-bdf9-e648aeeee082)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



