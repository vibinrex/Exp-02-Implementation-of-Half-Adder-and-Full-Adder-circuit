```
nmae:A.vibin rex
Reg no:23012635 
```
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
### Half Adder
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
## Fuller Adder
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
### TRUTH TABLE 

Half Adder circuit


![Ex-3 half adder table](https://github.com/vibinrex/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167280/b02607bc-e1dd-48d8-a8f0-d770f7f9f286)


Full Adder circit


![Ex-3 full adder](https://github.com/vibinrex/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167280/6a27866d-c308-4e25-be1d-5b6d82f9a8d1)



### RTL

Half Adder circuit


![Ex-3 half adder RTL](https://github.com/vibinrex/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167280/67fd4d2d-8e88-4b3e-a231-d85090807512)


Full Adder circit



![Ex-3 fuller ](https://github.com/vibinrex/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167280/8a676568-e445-4b94-8feb-1e0ac9157ae3)


### Output:


Half Adder Timing Diagram


![Ex-3 half adder diagram](https://github.com/vibinrex/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167280/087ee977-0ff4-43cb-83e2-f8e039159220)


Full Adder Timing Diagram


![Ex-3 full adder diagram](https://github.com/vibinrex/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167280/e46fbc71-c77d-471d-a8dd-e884769b383a)

### Result:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
