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
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SANJAY.T
RegisterNumber:212222110039
### HALF ADDER
module exp03(A,B,c,s);
input A,B;
output s,c;
assign s=A^B;
assign c=A&B;
endmodule
### FULL ADDER
module exp03(A,B,c,sum,carry);
input A,B,c;
output sum,carry;
assign sum=A^B^c;
assign carry=((A&B)|(B&c)|(c&A));
endmodule
```
Logic symbol & Truthtable
RTL realization

### Output:

### HALF ADDER RTL

![Screenshot de 03](https://github.com/sanjaythiyagarajan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119409242/9634dd29-76e3-4de6-a075-f7ab2adc0d7f)

### HALF ADDER WAVEFORM

![Screenshot 03 de](https://github.com/sanjaythiyagarajan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119409242/74c94ec0-79d2-407a-9100-33c0a3843e99)

### HALF ADDER TRUTH TABLE 

![WhatsApp Image 2023-09-01 at 09 21 03](https://github.com/sanjaythiyagarajan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119409242/2d293c52-c6c1-4bd8-b7b4-f548d52e1523)

### FULL ADDER RTL

![Screenshot 011 de 03 ](https://github.com/sanjaythiyagarajan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119409242/7c2c149b-1d5d-4609-a385-2af1a8afbc7a)

### FULL ADDER WAVEFORM

![Screenshot 01 de 03](https://github.com/sanjaythiyagarajan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119409242/be6ebad6-10b9-4dc7-8637-93593e364ab4)

### FULL ADDER TRUTH TABLE 

![WhatsApp Image 2023-09-01 at 09 21 06](https://github.com/sanjaythiyagarajan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119409242/44492473-fd74-4eb1-861e-19a51e9473d5)

### Result:

Thus the half adder and full adder circuits are designed and the truth tables is verified using quartus software.
