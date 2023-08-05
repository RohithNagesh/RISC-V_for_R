# RISC-V_for_R
The RISC-V instruction set architecture (ISA) is an open-source and royalty-free architecture designed for computer processors. It follows the Reduced Instruction Set Computing (RISC) principles, which aims to have a simple and efficient design. RISC-V was initially developed at the University of California, Berkeley in 2010 and has gained significant attention and adoption in both academic and commercial settings.

RV32I can be divided into six basic instruction formats. R-type instructions for register-register operations, an I-type instructions for immediate and load operations, and S-type instructions for store operations. B-type instructions for conditional branch operations. U-type instructions for long immediate and J-type instructions for unconditional jumps.

In this repository we write a systemverilog code for RISC-V 32bit proceessor which can execute only R-type instruction. And also a textbench to verify the processor code

# RISC-V R-type instruction format

R-type is an operation without immediate

The length of a binary instruction is 32bit

The 7 bits from 0 to 6 are opcode (operation code), used to identify the type of instruction. Bits 7 to 11 are the index of the rd register. The Rd register is also called the destination register, and the destination register is the register used to store the result. rs1 and rs2 are called source registers. In most cases, instructions need to read the values of the two source registers for operations. The index of rs1 is in bits 15-19, and the index of rs2 is in bits 20-24. The following is an example of how to use the register index

![image](https://github.com/RohithNagesh/RISC-V_for_R/assets/103078929/f1158c56-cbb8-4d6c-aa98-72a4d5ddd76e)

# DATAPATH (R-TYPE)
![image](https://github.com/RohithNagesh/RISC-V_for_R/assets/103078929/d8484f29-7eb2-4c07-9c0a-98635bf87604)

# TRUTH TABLE FOR CONTROL UNIT
![image](https://github.com/RohithNagesh/RISC-V_for_R/assets/103078929/2f4d4857-4aad-410a-8832-e8bc6f771953)

# Output screenshot
![image](https://github.com/RohithNagesh/RISC-V_for_R/assets/103078929/5a43539f-649a-439e-b59a-bb896b2868ae)


