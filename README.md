# VHDL Implementation of International Data Encryption Algorithm (IDEA) for FPGA

## Overview
This project implements the International Data Encryption Algorithm (IDEA) using VHDL for symmetric encryption and decryption. The design is tailored for FPGA hardware, providing a robust and efficient solution for secure data transmission. The implementation covers the complete IDEA algorithm, including its eight encryption rounds, and integrates core operations like bitwise XOR, addition modulo \(2^{16}\), and multiplication modulo \(2^{16} + 1\).

## Features
- **Symmetric Encryption**: Provides encryption and decryption functionalities using the IDEA algorithm.
- **Eight Rounds of Encryption**: Implements the full cycle of the IDEA algorithm with all necessary operations.
- **FPGA Compatibility**: Designed for efficient execution on FPGA hardware, ensuring high performance and low latency.
- **VHDL Simulation**: Includes testbenches for validating the implementation and ensuring functionality.

## Workflow
1. **Algorithm Overview**: The IDEA algorithm consists of eight rounds of processing with specific operations to secure data.
2. **VHDL Implementation**: Developed VHDL modules for each round of encryption and the necessary operations.
3. **Simulation**: Created testbenches to simulate and verify the functionality of the VHDL implementation.
4. **FPGA Synthesis**: The design is optimized for synthesis on FPGA devices, providing real-time encryption/decryption capabilities.

## Implementation Details
- **Key Operations**:
    - Bitwise XOR for combining data.
    - Addition modulo \(2^{16}\) for key mixing.
    - Multiplication modulo \(2^{16} + 1\) for data transformations.

- **Modules**:
    - `idea.vhdl`: Main VHDL implementation of the IDEA algorithm.
    - `testbench.vhdl`: Simulation and validation of the IDEA implementation.

## Installation and Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/TheMechanicHulk/IDEA_VHDL_Implementation.git
    cd IDEA_VHDL_Implementation
    ```

2. **Simulation Environment**:
    - Use a VHDL simulation tool such as ModelSim or GHDL to simulate and verify the implementation.
    - Compile and run the testbench:
    ```bash
    vhdl-compiler testbench.vhdl
    vhdl-simulator testbench
    ```

## Project Structure
```bash
├── src/               # Contains the VHDL source code
│   ├── idea.vhdl      # VHDL implementation of the IDEA algorithm
│   └── testbench.vhdl # Testbench for simulation
├── docs/              # Documentation and design details
└── README.md          # Project documentation
