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
```
Half Adder:
module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule


Full Adder:
module sub (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: B.VIJAY KUMAR
RegisterNumber: 212222230173
*/
Logic symbol & Truthtable
RTL realization
```



### Output:

### RTL
## Half Adder:
![Screenshot (307)](https://user-images.githubusercontent.com/119657657/233271657-9da79c6b-a6e3-47e4-ac19-502613b6339c.png)

## Full Adder:
![Screenshot (310)](https://user-images.githubusercontent.com/119657657/233271951-b1d3bb71-771a-4786-9efc-7bc302f7feb0.png)



### TIMING DIAGRAM
## Half Adder:
![Screenshot (308)](https://user-images.githubusercontent.com/119657657/233272108-62ca696c-d38a-4fb5-98c4-4675baeaf15e.png)
## Full Adder:
![Screenshot (311)](https://user-images.githubusercontent.com/119657657/233272247-2d7166f8-ec26-47ee-b9f1-c9e782673e46.png)


### TRUTH TABLE 
## Half Adder:

![image](https://user-images.githubusercontent.com/119657657/233272444-3bd0baab-b550-48eb-ba28-176f29b44fef.png)

## Full Adder:

![image](https://user-images.githubusercontent.com/119657657/233272496-097851c5-a5d5-4e8a-bd71-6dd96421eddb.png)




### Result:
Implementation of HalfAdder and FullAdder is completed sucessfully.
