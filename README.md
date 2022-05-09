# Experiment--04-Implementation-of-combinational-logic-using-universal-gates-
 ## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.


F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate


F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate


## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 
 
 Software – Quartus prime
## Theory:

A universal gate is a logic gate which can implement any Boolean function without the need to use any other type of logic gate. The NOR gate and NAND gate are universal gates. This means that you can create any logical Boolean expression using only NOR gates or only NAND gates. In practice, this is advantageous since NOR and NAND gates are economical and easier to fabricate than other logic gates. Similarly, an OR gate is typically realised as a NOR gate followed by an inverter.


## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.


## Program:
```
Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
Developed by: Jithendra V.A
RegisterNumber:  212221230043


NAND GATE PROGRAM:

module un1(a,b,c,d,f);
input a,b,c,d;
output f;
assign  f=((~(~c&b&a))&(~(~d&c&a))&(~(c&(~b)&a)));
endmodule


```

## Output:


## Truthtable(F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate)

![WhatsApp Image 2022-05-08 at 5 50 26 PM](https://user-images.githubusercontent.com/94154683/167332114-9e933a47-e145-4112-89f0-9eebf2a115d8.jpeg)


##  RTL realization(F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate)

![ex4 1](https://user-images.githubusercontent.com/94154683/167334936-06c1ba35-52f3-48a9-be5a-af9995e151e3.jpeg)

## Timing diagram(F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate)
![WhatsApp Image 2022-05-07 at 9 47 31 AM](https://user-images.githubusercontent.com/94154683/167332078-cb41acfb-4a3c-4355-b313-4183af3935a5.jpeg)


## Program:
```
Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
Developed by: Jithendra V.A
RegisterNumber:  212221230043


NOR GATE PROGRAM:
module nor1(a,b,c,d,f);
input a,b,c,d;
output f;
assign  f=(~(~((c&(~b)&a)|(d&(~c)&a)|(c&(~b)&a))));
endmodule

```
## Truthtable(f=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' USING NOR GATE)
![ex4](https://user-images.githubusercontent.com/94154683/167334723-2a3b8fd3-17f7-40ea-9dc0-d85ba964a01c.png)


##  RTL realization(f=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'USING NOR GATE)


![WhatsApp Image 2022-05-07 at 7 00 39 PM](https://user-images.githubusercontent.com/94154683/167332030-767efe56-cb16-4de0-90db-664f3c5df6f7.jpeg)

## Timing diagram (f=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'USING NOR GATE)


![WhatsApp Image 2022-05-07 at 9 47 31 AM (1)](https://user-images.githubusercontent.com/94154683/167332093-0ff4add8-3895-4204-afed-f10780583a1b.jpeg)

## Result:
The given logic function is implemented using NAND and NOR gates and it is verified successfully in Quartus using Verilog programming.
