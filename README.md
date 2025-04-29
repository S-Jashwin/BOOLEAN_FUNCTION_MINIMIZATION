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

module funct1(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule

module funct2(w,x,y,z,f2); 
input w,x,y,z; 
output f2; 
assign f2=((~y & z)|( w & y )|(x & y)); 
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:JASHWIN.S

RegisterNumber:212224040131*/


**RTL realization**



![image](https://github.com/user-attachments/assets/35834e1b-9047-46a4-8399-eca92b87f3f1)


***TRUTH TABLE***

![image](https://github.com/user-attachments/assets/73307072-61d0-44cf-8bd0-151f131bbbdf)


![image](https://github.com/user-attachments/assets/7f7e755d-c423-486c-a61a-ba13e1a02f72)


**Timing Diagram**


![image](https://github.com/user-attachments/assets/c780038f-1001-4221-a105-dd4cfaae51e0)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

