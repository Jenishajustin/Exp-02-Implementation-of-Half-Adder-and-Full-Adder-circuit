# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: JENISHA.J
RegisterNumber:  212222230056

HALF ADDER

module ha (a,b,s,c);
input a,b;
output s,c;
xor(s,a,b);
and(c,a,b);
endmodule

FULL ADDER

module Fa (a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor (d,a,b);
xor (s,d,ci);
and (e,d,ci);
and (f,a,b);
or (co,e,f);
endmodule
```
#### Logic symbol:
##### HALF ADDER
![HA (2)](https://user-images.githubusercontent.com/119405070/232263882-d38176bb-0fb8-437a-876c-6947192b2029.png)

##### FULL ADDER
![FA logic gate](https://user-images.githubusercontent.com/119405070/232263832-9c7998af-e258-44aa-b3d7-02ba1afda309.png)

### Output:
### RTL
##### HALF ADDER
![ha1](https://user-images.githubusercontent.com/119405070/232263905-2a950372-7b55-4caf-88c6-b2b9863e71c5.png)

##### FULL ADDER
![Fa logic dia](https://user-images.githubusercontent.com/119405070/232263930-faec0f9c-ac9b-448d-bd54-95ae6c83c378.png)

### TIMING DIAGRAM
##### HALF ADDER
![ha3](https://user-images.githubusercontent.com/119405070/232264089-0122eddf-e585-42d7-bd17-248a58479f2d.png)

##### FULL ADDER
![Fa out](https://user-images.githubusercontent.com/119405070/232263958-19bd9bbd-c2e2-4787-8a1b-8cf62226502a.png)

### TRUTH TABLE 
##### HALF ADDER
![ha truth](https://user-images.githubusercontent.com/119405070/232264160-7f805ad9-653e-482e-abe9-fb34d55efe8d.png)

##### FULL ADDER
![fa truth](https://user-images.githubusercontent.com/119405070/232264248-14515873-fce4-4bc8-8127-4233443b32e2.png)

### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
