Multi-Cycle Risc-V Processor
This project is a computer architecture design that implements a multi-cycle processor with a custom instruction set and an accumulator-based datapath. The main goal is to reduce execution cycle count by moving data efficiently between registers and the ALU, while supporting a compact memory model and multiple instruction categories.

Overview
The processor is designed as a multi-cycle system, meaning each instruction is executed in multiple stages rather than in a single long cycle. This makes the architecture more efficient and modular, especially for complex operations such as memory access, arithmetic processing, and branching.

Architecture
Word size: 16-bit
Memory: 16K × 4 bits
Processor style: Multi-cycle, register-based
Core idea: Use an accumulator to simplify execution and reduce the number of cycles
ALU: Supports 6 operations:
Add
Subtract
AND
OR
NOT
Pass/Move
Instruction Set
The instruction set is divided into 4 types:

Type A
Memory and control flow instructions:

Load
Store
Jump
Type B
Conditional control instruction:

BranchZ
Type C
Register and ALU operations:

MoveTo
MoveFrom
Add
Sub
And
Or
Not
Nop
Type D
Immediate operations:

Addi
Subi
Andi
Ori
Purpose
This design demonstrates how a custom processor can be organized around:

instruction decoding,
control signal generation,
ALU execution,
memory interaction,
and conditional branching.
