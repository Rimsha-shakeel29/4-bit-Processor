# 4-bit-Processor
Digital Logic Design Project 1

This project is implemented in LogicWorks. It is a 4-bit processor which consists of 4 data registers each of 4 bits and an instruction register (IR) of 7 bits. The first 3 bits of the instruction tells which operation is to be performed, the next 2 bits signifies the first register and the last two bits signifies the second register.


I6-I4	                I3-I2	                                I1 – I0

Operation Code	      4-bit register operand 1(R1)           4-bit register operand 2 (R2)

The following operations are performed by the processor.


Operation Code	        Operation Performed	          Description

000	                   R1 = A	                       Load the contents of input A in to the register operand 1.

001	                   R1 = R2	                      Move the contents of register operand 2 in to register operand 1.

010                    R1 = R1 + R2	                 Add the contents of register operand 1 and register operand 2 and load in register operand 1.

011	                    R1 = R1 - R2	                Subtract the contents of register operand 2 from register operand 1 and load in register operand 1.
 
100	                    R1 = R1 * R2	                Multiply the contents of register operand 1 and register operand 2 and load in register operand 1 and 2. (As the result is of 8 bits)

101	                   R1 = R1/2i	                    Divide the register contents of register operand 1 with 2i (i is an input) and load the result in register operand 1.

110	                    R1 = R1*2I	                   Multiply the register contents of register operand 1 with 2i (i is an input) and load the result in register operand 1.

111	                     R1 = R1 + R2	                Logical OR the contents of register operand 1 and register operand 2 and load in register operand 1.

Inputs:

Clock Pulse (CP), 7-bits Instruction, A, i

Output:

Contents of each register
 
