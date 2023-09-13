# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: MAHESWARAN.K
RegisterNumber:  212222110023

module EX2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire X1,X2,X3,X4,X5;
assign X1=(~A)&(~B)&(~C)&(~D);
assign X2=(A)&(~C)&(~D);
assign X3=(~B)&(C)&(~D);
assign X4=(~A)&(B)&(C)&(D);
assign X5=(B)&(~C)&(D);
assign F1=X1|X2|X3|X4|X5;
endmodule

```
## Truth Table:
![263468886-13f060b0-a236-4fce-9853-4942dcf3eaff](https://github.com/22009011/Experiment--02-Implementation-of-combinational-logic-/assets/118343461/2e48a858-37e8-4113-b815-65fa3518e54a)

## RTL realization:
![ex02 digitalScreenshot 2023-08-27 152926](https://github.com/22009011/Experiment--02-Implementation-of-combinational-logic-/assets/118343461/34db92b0-08be-4768-ad14-01eee3bba259)

## Output wave form:
![263468736-9a41696f-fece-4e17-bdf6-9f37a5a6e51a](https://github.com/22009011/Experiment--02-Implementation-of-combinational-logic-/assets/118343461/fdc0fbb6-fe3e-4623-b104-a67bcdf6cc77)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
