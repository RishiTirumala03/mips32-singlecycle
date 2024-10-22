# 32-Bit Single Cycle MIPS Processor

This repository contains the design and implementation of a 32-bit single cycle MIPS processor, developed as part of the EECS 112L class at the University of California, Irvine (UCI). The project aims to provide a clear understanding of digital logic design and computer architecture.

## Table of Contents

- [Features](#features)
- [Architecture](#architecture)
- [Implementation](#implementation)
- [Usage](#usage)
- [Simulation](#simulation)
- [License](#license)
- [Contributors](#contributors)

## Features

- 32-bit instruction set architecture (ISA)
- Single cycle execution for all instructions
- Support for:
  - Arithmetic operations (ADD, SUB, etc.)
  - Logical operations (AND, OR, etc.)
  - Data transfer instructions (LW, SW)
  - Control flow instructions (BEQ, JUMP)
- Basic support for immediate values
- Register file with 32 registers

## Architecture

The processor architecture follows the classic MIPS design. It consists of the following major components:

- **Instruction Memory**: Holds the program instructions.
- **Data Memory**: Stores the data used by the program.
- **ALU (Arithmetic Logic Unit)**: Performs arithmetic and logical operations.
- **Register File**: Contains the 32 general-purpose registers.
- **Control Unit**: Decodes the instructions and generates control signals.


## Implementation

The processor is implemented using Verilog, and the design follows a modular approach, allowing easy modifications and extensions. Key modules include:

- `alu.v`: ALU operations
- `register_file.v`: Register file management
- `control_unit.v`: Control signal generation
- `data_memory.v`: Data memory operations
- `instruction_memory.v`: Instruction fetching

## Usage

To synthesize and simulate the MIPS processor, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/username/mips-processor.git
   cd mips-processor
2. Test the Processor:
   A basic testbench is included in the testbench directory to verify the functionality of the processor.
