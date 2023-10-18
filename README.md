# Experiment--02-Implementation-of-combinational-logic
 
## AIM:
Implementation of combinational logic gates.
To implement the given logic function verify its operation in Quartus using Verilog programming.
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.


## Logic Diagram
## Procedure
## Program:
Developed by: ARHAM S
RegisterNumber: 212222110005

```
module proj2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1 = (~A)&(~B)&(~C)&(~D);
assign x2 = (A)&(~C)&(~D);
assign x3 = (~B)&(C)&(~D);
assign x4 = (~A)&(B)&(C)&(D);
assign x5 = (B)&(~C)&(D);
assign F1 = x1+x2+x3+x4+x5;
endmodule
```
## Output:
## RTL
![1](https://github.com/Sriram8452/Experiment--02-Implementation-of-combinational-logic-/assets/118708032/8126d148-2994-4635-af11-af3f3868509b)

## Truth Table
![2](https://github.com/Sriram8452/Experiment--02-Implementation-of-combinational-logic-/assets/118708032/3a3e0e8c-d18e-410e-84b6-ed6ddfc1b0ab)

## Timing Diagram
![3](https://github.com/Sriram8452/Experiment--02-Implementation-of-combinational-logic-/assets/118708032/5b4efcc0-aad7-4608-938c-d34940cf1d23)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
