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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/ 212221230078 Name: Praneet S
```

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
```


**Logic Symbol and Truth table**
![image](https://github.com/user-attachments/assets/d96e0963-20b6-4d9b-abe9-36fe125b89b2)
![image](https://github.com/user-attachments/assets/9c703529-7af3-43d2-9a7e-ba130f14042d)



**RTL realization Output:**
![image](https://github.com/user-attachments/assets/4ec52617-10f9-46fe-bb25-c560387d8cec)
![image](https://github.com/user-attachments/assets/78225d9d-219a-4a70-aa3b-272bc9c0d359)



**RTL**
![image](https://github.com/user-attachments/assets/571d779d-5bbf-4f8f-b040-ce6f180bca29)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
