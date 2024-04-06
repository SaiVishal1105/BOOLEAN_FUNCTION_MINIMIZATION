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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by: SAI VISHAL D
RegisterNumber: 212223230180
module Booleanfunction_2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u,v,w1,w2,x1,x2,y1,y2,z1,z2;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
and(w1,a,b,c);
and(w2,~a,~b,~c);
or(f2,w1,w2);
endmodule 
```
**RTL**
![Screenshot 2024-04-01 193443](https://github.com/SaiVishal1105/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742557/5e7b2da6-a227-4d07-a7b6-bcd4372122a2)

**Timing Diagram**
![Screenshot 2024-04-06 132325](https://github.com/SaiVishal1105/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742557/241b62dc-9436-4053-ac84-cb20aaed51e7)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

