## NAME: F.FRANKLIN
## REG NO:24900641
# EXPERIMENT 2- BOOLEAN FUNCTION  IMPLEMENTATION  
# BOOLEAN_FUNCTION_MINIMIZATION

# AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

# Equipment Required:

Hardware – PCs, Cyclone II , USB flasher </br>
Software – Quartus prime

# Theory
Implementing Boolean functions in Verilog HDL (Hardware Description Language) involves translating the simplified Boolean expressions into Verilog code to describe the behavior of digital circuits. The basic building blocks in Verilog is module. The module represent a combinationa circuit. Use logical operators (&, \, ~, ^) to implement Boolean functions directly. Use built-in gate primitives for basic functions: Use University program VWF to verify the functionality of your Verilog modules. Create waveform and check outputs against expected results.


# Procedure

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


# Program:

#### Developed by: RegisterNumber:*/
#### module booleanfunction(a,b,c,d,F1,F2,w,x,y,z);
#### input a,b,c,d,w,x,y,z;
#### output F1,F2;
#### wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
#### assign x1=(~a)&(~b)&(~c)&(~d);
#### assign x2=(a)&(~c)&(~d);
#### assign x3=(~b)&(~c)&(~d);
#### assign x4=(~a)&(b)&(c)&(d);
#### assign x5=(b)&(~c)&(d);
#### assign x6=(x)&(~y)&(z);
#### assign x7=(~x)&(~y)&(z);
#### assign x8=(~w)&(x)&(y);
#### assign x9=(w)&(~x)&(y);
#### assign x10=(w)&(x)&(y);
#### assign F1=x1|x2|x3|x4|x5;
#### assign F2=x6|x7|x8|x9|x10;
#### endmodule

# TRUTH TABLE
![WhatsApp Image 2024-11-04 at 11 43 35_c12123e7](https://github.com/user-attachments/assets/3b67d9e5-cc1c-4b83-add8-945c09b14e06)

# RTL
![Screenshot (4)](https://github.com/user-attachments/assets/578981f4-0690-4a35-bfe9-cab79d96036e)


# Timing Diagram
![WhatsApp Image 2024-11-04 at 11 28 24_1ea4e137](https://github.com/user-attachments/assets/825dc4f9-9620-4810-9c7a-0dccbba4f026)

# Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

