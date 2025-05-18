

*AIM:*

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

*Equipment Required:*

Hardware – PCs, Cyclone II , USB flasher

*Software – Quartus prime*

*Theory*

*Logic Diagram*

FUNCTION 1 K-MAP:

![Screenshot 2025-04-23 212204](https://github.com/user-attachments/assets/fff474d9-6fe1-424d-b5ba-b6444c8f593c)

FUNCTION 2 K-MAP:

![Screenshot 2025-04-23 212216](https://github.com/user-attachments/assets/06f8cb51-f033-47fb-b4e9-b55ff6adcfe4)



*Procedure*

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


*Program:*



 FUNCTION 1:

 module function1(a,b,c,d,f1);
 input a,b,c,d;
 output f1;
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 endmodule

 FUCTION 2:

 module funct2(w,x,y,z,f2);
 input w,x,y,z;
 output f2;
 assign f2=((~y & z)|( w & y )|(x & y));
 endmodule



FUNCTION 1:


![Screenshot 2024-12-08 214517](https://github.com/user-attachments/assets/1d07ede7-c7f7-4db2-9509-d8120929dc72)

FUNCTION 2:

![Screenshot 2024-12-08 214526](https://github.com/user-attachments/assets/3042b310-372a-406a-81c5-f9e8967a2b33)




Developed by:AAKIL AHAMED S
RegisterNumber:212224040002



*RTL realization*

*Output:*

*RTL*

FUNCTION 1:

![Screenshot 2024-12-08 214718](https://github.com/user-attachments/assets/2f9524a5-b738-4af8-b4f2-2836902b789a)

FUNCTION 2:

![Screenshot 2024-12-08 214722](https://github.com/user-attachments/assets/4ff42f59-5c9b-444f-94c9-2b4100f09b86)


*Timing Diagram*

FUNCTION 1:

![Screenshot 2024-12-08 214851](https://github.com/user-attachments/assets/1ca11228-6830-4995-9d45-1a0de0093cea)


FUNCTION 2:

![Screenshot 2024-12-08 214900](https://github.com/user-attachments/assets/fe854bb8-d7a7-44fb-9869-14b0b571d16f)

*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
