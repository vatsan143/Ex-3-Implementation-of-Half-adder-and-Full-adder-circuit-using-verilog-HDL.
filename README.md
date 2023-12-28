# Date:
# Ex - 3 Implementation of Half adder and Full adder circuit using verilog HDL

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
Developed by: Srivatsan G
RegisterNumber:  23013933

half_adder:
module half_adder(a,b,s,c);
output s,c;
input a,b;
assign s=a^b;
assign c=a&b;
endmodule

full_adder:
module full_adder(A,B,cin,S,cout);
input A,B,cin;
output S,cout;
assign S=A^B^cin;
assign cout=(A&B)| (B&cin)| (A&cin);
endmodule
*/
Logic symbol & Truthtable
RTL realization

### Output: 
half_adder: 
![3](https://github.com/sanjayy2431/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365143/9c9936b0-dc5d-4398-a96a-93972d171e0a) 
full_adder:
![image](https://github.com/sanjayy2431/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365143/e0b6d8b2-f057-4d72-9f5f-607bc401b9d2)


RTL:
half_adder:
![image](https://github.com/sanjayy2431/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365143/b3937af4-a008-48f1-99d0-3ce41af1dac2)
full_adder:
![image](https://github.com/sanjayy2431/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365143/546d956d-2dbc-415b-a9b9-1b33c6984127)




### TIMING DIAGRAM


### TRUTH TABLE 
## half_adder:

![image](https://github.com/sanjayy2431/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365143/180902e3-bd62-4591-a56a-5c28f1bb8b04)




## full_adder:

![image](https://github.com/sanjayy2431/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365143/dfcb2a12-1b86-445d-8dcb-9594f1c16a3b)



### Result:

The program half adder and full adder executed succesfully.
