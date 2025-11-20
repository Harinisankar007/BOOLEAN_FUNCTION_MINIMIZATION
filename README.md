# BOOLEAN_FUNCTION_MINIMIZATION
### Date:30-09-2025
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

Developed by: HARINI S
RegisterNumber: 212224240049*/
```
module Boolean(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
**RTL**
<img width="556" height="942" alt="image" src="https://github.com/user-attachments/assets/d6d79d9a-1c58-4b18-94b3-72822f68c7dd" />

**RTL realization**
![image](https://github.com/user-attachments/assets/6b38ca0a-f8e3-4ae3-9252-2452fbbc1218)
<img width="675" height="997" alt="image" src="https://github.com/user-attachments/assets/5557b508-9558-40bf-b73c-6fe529f3ab0f" />

**Timing Diagram**

![image](https://github.com/user-attachments/assets/100994ba-2251-4bf0-a9f5-85052373d08c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

