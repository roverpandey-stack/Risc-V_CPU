# Risc-V_CPU
## Overview

This project implements a single-cycle 32-bit CPU based on a RISC-style architecture. The processor is designed to execute each instruction in a single clock cycle, making it simple and easy to understand for educational purposes.

The CPU integrates all the fundamental components of a processor, including the Program Counter, Instruction Memory, Register File, ALU, Data Memory, Control Unit, and Sign/Zero Extender.

## Features

32-bit architecture

Single-cycle execution (each instruction completes in one cycle)

Supports arithmetic, logical, memory, and control flow instructions

Modular design with separate components for easy understanding and debugging

Can be extended to support pipelining in future versions

## Components

The CPU consists of the following main components:

1. Program Counter (PC) – Holds the address of the current instruction.

2. Instruction Memory – Stores the instruction set.

3. Register File – Contains 32 general-purpose registers for operand storage.

4. Arithmetic Logic Unit (ALU) – Performs arithmetic and logical operations.

5. Data Memory – Used for load and store instructions.

6. Control Unit – Generates control signals for instruction execution.

7. Sign/Zero Extender – Extends immediate values to 32 bits.

8. Multiplexers (MUXes) – Used for instruction/data path selection.

9. Adder – For PC update and branch calculations.

10. Instruction Decoder – Interprets opcode and generates signals.

## Instruction Set

This CPU supports a simplified instruction set including:

Arithmetic/Logical: ADD, SUB, AND, OR, XOR, SLT

Memory: LW, SW

Control Flow: Branch, JUMP, conditional branch

## Implementation Details

Data Path Width: 32-bit

Instruction Length: 32-bit

Cycle per Instruction: 1 (Single-Cycle)

Design Language: Verilog

Simulation Tool: ModelSim and Quatrus prime

## Getting Started

Clone the repository:

git clone https://github.com/your-username/single-cycle-32bit-cpu.git


Open the project in your HDL simulation tool.

Compile and run the design.

Load a sample instruction memory file (instructions.mem) and observe CPU execution in the waveform/simulation.

## Project Structure
single-cycle-32bit-cpu/
│── src/                # HDL source files (CPU modules)
│── testbench/          # Testbench files
│── docs/               # Documentation, block diagrams
│── instructions/       # Sample instruction memory files
│── README.md           # Project overview

## Block Diagram

(Insert your CPU datapath diagram here for clarity)

## Testing

Unit-tested each component (ALU, Register File, Control Unit).

Verified end-to-end instruction execution with sample programs.

## Future Work

Extend instruction set (e.g., MUL, DIV, BNE).

Add pipeline stages (IF, ID, EX, MEM, WB).

Hazard detection and forwarding mechanisms.

Implement a cache for memory operations.

## Contributors  
- [Divyansh Pandey](https://github.com/roverpandey-stack)  
- [Kritika Parihar](https://github.com/Kritika-Parihar-20234091)  
