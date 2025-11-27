# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Truth Table**

<img width="503" height="220" alt="image" src="https://github.com/user-attachments/assets/45fec5b2-b1c4-44d8-922d-ecdaf10099e1" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```

**Developed by:**

Janesha S

**RegisterNumber:**

25018817

**RTL logic**

<img width="1920" height="1080" alt="Screenshot (141)" src="https://github.com/user-attachments/assets/1fbda5a3-fa40-479f-872e-4571916463cc" />

**Timing Diagram**

<img width="1920" height="1080" alt="Screenshot (149)" src="https://github.com/user-attachments/assets/566edd12-1b21-4622-882f-941325b5d88e" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

