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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Maatheshwar B
RegisterNumber:25017484
```
```
module experiment2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module experiment2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**


<img width="1040" height="515" alt="image" src="https://github.com/user-attachments/assets/44f7adbb-1c53-4b31-ab45-01cda671c5ff" />


<img width="930" height="498" alt="image" src="https://github.com/user-attachments/assets/0a6af679-52a7-4363-83af-c82a529a977c" />




**Timing Diagram**

<img width="1066" height="585" alt="image" src="https://github.com/user-attachments/assets/fd2aa960-f9bd-4ecc-b047-3703dd272f9e" />

<img width="1076" height="605" alt="image" src="https://github.com/user-attachments/assets/5afd7891-ae2f-4bae-881d-ec886a706020" />

**Result:**


Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

