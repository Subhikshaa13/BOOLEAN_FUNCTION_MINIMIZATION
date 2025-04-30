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

Developed by: Subhikshaa m RegisterNumber: 212222230151 */
module exp02(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

**RTL realization**
![437948055-8aa30fe0-7c27-4287-884a-4681af375eb1](https://github.com/user-attachments/assets/62ce1189-536b-4621-a5be-2022abea55f5)
Truth Table
![437937368-573ec45c-4bfc-4f33-807d-9a2f329b4bc3](https://github.com/user-attachments/assets/ff7c5eb4-d176-4946-b5d4-3e1219afa30d)
![437937380-2bd81f87-d436-4213-bc25-7295fce11a71](https://github.com/user-attachments/assets/ff3e8ba0-17fb-4b55-95d9-df604ec03570)
Timing Diagram
![437948085-f323a383-d456-455f-98f5-7909d4e4ee00](https://github.com/user-attachments/assets/daccc869-24fd-4408-827e-6dc39d3997a5)
**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
