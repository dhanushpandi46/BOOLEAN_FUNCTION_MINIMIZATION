# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);

input A,B,C,D,W,X,Y,Z;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

output F1,F2;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule
Developed by: RegisterNumber:*/  dhanushpandi   24012399


**RTL realization**
![logic diagram](https://github.com/user-attachments/assets/37827230-4776-45aa-85e2-e30b32ff2691)

**logic sympol & truth table**
![truth table](https://github.com/user-attachments/assets/ac97dfa3-6464-4366-9d97-f279a0964a65)
![truth table 2](https://github.com/user-attachments/assets/43c53853-1019-49ee-8596-06c7d1810a10)


**Output:**
![output](https://github.com/user-attachments/assets/c1b9b958-e041-49ff-af6c-7091fe49f83a)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

