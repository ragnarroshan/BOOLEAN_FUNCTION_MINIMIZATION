# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module ex02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
**RTL realization**



**Output:**

**RTL**



![kirthick roshan exp 2 rtl](https://github.com/ragnarroshan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147474287/5e4751a8-a43f-432c-897d-1139edf0be91)

**Timing Diagram**

![exp 2 truth table](https://github.com/ragnarroshan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147474287/e92fad09-10c9-4697-8e8f-4d4c39f4d9e0)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

