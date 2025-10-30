# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

<img width="428" height="318" alt="image" src="https://github.com/user-attachments/assets/bd32d028-7e6f-48fb-b634-3104002778b1" />
<img width="608" height="622" alt="image" src="https://github.com/user-attachments/assets/4f2db67a-5c3f-49dd-947f-67c388bb70d4" />



**Procedure**

Program to design a full adder and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
Developed by: h mohammed irfan 
RegisterNumber: 25006317


**Program:**

 module FAHA1 (a,b,c,x,y,z,sum,dif,car,bor); input a,b,c,x,y,z; output sum,dif,car,bor; assign sum = a^b^c; assign car = a&b |
 a&c | b&c; assign dif = x^y^z; assign bor = ~x&z | ~x&y | y&z; endmodule

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**

<img width="520" height="387" alt="image" src="https://github.com/user-attachments/assets/fd6bb49b-5fef-41e2-99b8-a8a57436a261" />


**Output Timing Waveform**

<img width="747" height="142" alt="image" src="https://github.com/user-attachments/assets/f36b66c2-7fa4-4736-a3aa-208b1bec04db" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



