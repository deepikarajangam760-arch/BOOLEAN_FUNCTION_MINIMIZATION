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
module exp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule 

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Deepika R RegisterNumber:25016530


**RTL realization**
<img width="1076" height="745" alt="image" src="https://github.com/user-attachments/assets/c9a63b61-252c-4461-8e9e-1e3a5b25aae9" />

**Output:**
<img width="1537" height="784" alt="image" src="https://github.com/user-attachments/assets/e672cb09-1f5b-4c25-a153-16c5261d7959" />



**RTL**
<img width="1443" height="879" alt="image" src="https://github.com/user-attachments/assets/9ef20451-1a58-466e-a19f-52dfbf76238d" />


**Timing Diagram**
<img width="1550" height="915" alt="image" src="https://github.com/user-attachments/assets/d65acb6d-55e2-484c-b26e-36e2a1b26efd" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

