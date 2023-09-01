```
Developed by : S.ROSELIN MARY JOVITA
Reg no : 212222230122
```
 # Exp-03 Implementation of Half Adder and Full Adder circuit

# Implementation of Half Adder and Full Adder circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

Theory
 
Adders are digital circuits that carry out addition of numbers.

### Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit

Switch ON the main switch

If the output is 1, then the led glows.

### Program:

/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
HALF ADDER

module electronics3 (A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule

FULL ADDER
module Digital3 (A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```
*/

Logic symbol

![image](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/926045f9-9728-45ae-b07c-d3b2d96477c4)


### Output:
#RTL

HALF ADDER

![DE3](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/43ca89f9-c6af-42e5-98c5-4dab182f16f5)

FULL ADDER

![Digital3 1](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/082a0a32-46ad-45a6-b73f-ef476e44d937)


### RTL  TRUTH TABLE 

 HALF ADDER
 
![image](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/39067e9e-2b1a-4771-aa5b-e5b3c25186b1)

FULL ADDER

![image](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/c3d2d013-2f31-40cf-b047-abfbc9f6e099)


## TIMING DIAGRAM

HALF ADDER

![DE EXP3](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/02ce4d1c-967d-4b4c-90b3-831db80ee8c0)



FULL ADDER


![Digital3](https://github.com/Roselinjovita/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119104296/4c4e19ff-ab59-4fc1-998d-92aa8904f19a)

 

### Result:

Thus the implementation of half adder and full adder circiut are stuided and the truth table for different logic gates
