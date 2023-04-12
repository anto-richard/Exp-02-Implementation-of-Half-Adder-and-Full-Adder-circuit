# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit...

# Implementation-of-Half-Adder-and-Full-Adder-circuit:

### AIM:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:

Hardware – PCs, Cyclone II ,

USB flasher,

Software – Quartus prime.

### Theory:

Adders are digital circuits that carry out addition of numbers.

### Half Adder:

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder:

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER :


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER :

### Procedure:

1)Connect the supply (+5V) to the circuit.

2)Switch ON the main switch.

3)If the output is 1, then the led glows.

### Program:

```c
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Anto Richard.S
RegisterNumber:  212221240005

HALF ADDER:

module HalfAdder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule 

FULL ADDER:

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

```

### Output:

### Half adder:


### Logic symbol:

![img 1](https://user-images.githubusercontent.com/93427534/231545788-96c58368-1617-47a9-ae2c-44a4653edfc3.png)



### RTL realization:

![img 2](https://user-images.githubusercontent.com/93427534/231545798-af2d542d-0059-4c64-a2e7-8b2e09bee291.png)


### Truthtable:

![img 3](https://user-images.githubusercontent.com/93427534/231545808-16a8d697-2e0c-4cba-8bbd-538bfb194641.png)


### TIMING DIAGRAM:

![img4](https://user-images.githubusercontent.com/93427534/231545827-75f34e4f-c2e9-435f-8cfd-519866c44a8a.png)


### Full adder:



### Logic symbol:

![img5](https://user-images.githubusercontent.com/93427534/231545838-9ff2363c-5678-4a10-9608-e72a1bb9d17e.png)


### RTL realization:

![img6](https://user-images.githubusercontent.com/93427534/231545853-4450e427-13fb-465c-8c1a-37106eb8832f.png)


### Truthtable:


![img7](https://user-images.githubusercontent.com/93427534/231545863-1ccff0b6-586c-4a25-beef-1b73b69933bf.png)

### TIMING DIAGRAM:

![img8](https://user-images.githubusercontent.com/93427534/231545880-338a1721-5fbd-46dd-b737-b99bfe913962.png)


### Result:

Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
