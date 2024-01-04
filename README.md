NAME:VIGNESH M<br>
REFERENCE NUMBER:212223040235

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

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/22f22fd3-2815-4e9e-86ef-861b9146a0ad)

#### Figure -01 HALF ADDER 

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/4f135316-84af-493b-adaf-fb4ad45c04b0)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows. 

Program:
# Half Adder:


module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule



# Full Adder


module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule



### TRUTH TABLE 
Half Adder Circuit:

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/d5343186-5d9a-4997-9342-a607059c7c34)

Full Adder Circuit:-

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/2632aff6-b9b7-4ef8-84d7-888159d36056)

### RTL
Half Adder Circuit:

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/1175ec6a-2dd3-48ee-b95f-15d0dfc70332)

Full Adder Circuit:-

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/62e01291-c556-4cd1-b58f-76dfa2fa5fd8)

### Output:
Half Adder Circuit:-

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/959e531c-9b47-4e1b-a9f1-c2c0af3168b1)

Full Adder Circuit:-

![image](https://github.com/Vignesh-M-07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151615193/6366a173-b575-40c2-a1e5-1fb0bfcad153)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
