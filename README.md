# NAME: YASEEN.F
# Reference No: 23014215
# Exp 02 Implementation of Half Adder and Full Adder circuit
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

## Program:
Half adder:
module exp3(sum, carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
full adder:
module fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule
RTL realisation:
Half Adder:
image

## RTL realization:
## HALF ADDER:
![image](https://github.com/YASEEN23014215/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365441/b23e3fb2-7bbd-48ee-b4e7-2d862fb31994)
## FULL ADDER:
![image](https://github.com/YASEEN23014215/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365441/f5377b14-5d2b-484a-8055-563123ad29b0)

### TIMING DIAGRAM:
## HALF ADDER:
![image](https://github.com/YASEEN23014215/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365441/9fd943dc-40c5-492d-a11a-2c8513d68845)
## FULL ADDER:
![image](https://github.com/YASEEN23014215/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365441/247629d9-0751-476c-bcb2-604c5e0907af)



### TRUTH TABLE:
## HALF ADDER:
![image](https://github.com/YASEEN23014215/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365441/6a565934-cab9-4921-af22-c08919ef1026)
## FULL ADDER:
![image](https://github.com/YASEEN23014215/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149365441/7d074776-a0d5-4fbf-9bb5-3614fb202e59)



### Result:
