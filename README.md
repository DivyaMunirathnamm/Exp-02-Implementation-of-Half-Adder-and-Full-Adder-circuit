# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
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
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Divya M
RegisterNumber: 2303162

```
module EX03DEHA(A,B,sum,carry);
input A,B;
output sum,carry;
xor(sum,A,B);
and(carry,A,B);
endmodule

module EX03DEFA(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=((a^b)^c);
assign carry=((a&b)|(b&c)|(c&a));
endmodule
```
*/

### RTL:
![Screenshot (183)](https://github.com/DivyaMunirathnamm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147474097/222bd6c2-3834-4285-9250-ab19ddd35cbb)
![Screenshot (185)](https://github.com/DivyaMunirathnamm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147474097/af300852-4844-4610-aa07-955f6caa2e5f)

### TIMING DIAGRAM
![Screenshot (184)](https://github.com/DivyaMunirathnamm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147474097/2eb7db63-d336-4c1d-b0cb-7e3c5127d27d)
![Screenshot (186)](https://github.com/DivyaMunirathnamm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147474097/6dd6c567-84f7-4644-934d-59af1bb12f91)

### TRUTH TABLE:
![Screenshot (188)](https://github.com/DivyaMunirathnamm/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147474097/b7218d22-cf0e-4739-b81c-5988e430b1d4)

### Result:
