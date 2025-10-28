## Custom RISC-V Processor

<img width="1029" height="610" alt="architecture" src="https://github.com/user-attachments/assets/a750da2b-7069-44df-817b-74dc7fcc36ed" />


Custom-designed 32-bit RISC-V processor developed using Verilog HDL. Built from the ground up as part of an educational and research-focused initiative, it supports the RV32I base instruction set and features a clean, modular, and pipelined architecture.

# RISC-V Processor Design Project

### Overview
This repository contains the complete design and implementation of a **RISC-V based processor** developed as part of the VLSI design learning and implementation phase.  
The goal of this project is to understand and build a **modular RISC-V CPU architecture** covering instruction fetch, decode, execute, memory, and write-back stages.

---

## Project Objectives
- Design a **32-bit RISC-V processor** in Verilog HDL.  
- Implement a modular structure including:
  - Program Counter and Instruction Memory
  - Register File
  - ALU (Arithmetic Logic Unit)
  - Control Unit
  - Sign Extension Unit
  - Data Memory
- Simulate the complete datapath and verify with testbenches.
---

## Architecture Overview
The RISC-V processor follows a **5-stage pipeline-like structure** :

1. **Instruction Fetch (IF)** – Fetches the instruction from memory.  
2. **Instruction Decode (ID)** – Decodes opcode, reads registers, and generates control signals.  
3. **Execute (EX)** – Performs ALU operations and branch evaluations.  
4. **Memory Access (MEM)** – Handles load/store operations.  
5. **Write Back (WB)** – Writes results back to the register file.

---

## Modules Implemented

| Module | Description | Status |
|--------|--------------|--------|
| **Program Counter** 
| **Instruction Memory** 
| **Register File** 
| **ALU** 
| **Sign Extension Unit** 
| **Control Unit** 
| **Data Memory** 
| **Top-Level Integration** 
| **Testbench**

---

## Features
- Implements **RISC-V RV32I** instruction set subset  
- Modular and reusable design  
- Parameterized Verilog modules  
- Synthesis-ready RTL  
- Testbench and waveform verification  
- Compatible with FPGA prototyping  

---

## Tools & Technologies
- **HDL:** Verilog  
- **Simulator:** Vcs / iverilog  
- **Synthesis:** Synopsys Design Compiler  / yosys
- **Backend (Future):** ICC2 / OpenROAD 
- **Documentation:** Markdown + GitHub  

---

## Repository Structure



### References

- RISC-V Official Specs: https://riscv.org/specifications/
- FPGA: PYNQ-Z2 Board: https://www.tul.com.tw/ProductsPYNQ-Z2.html
- RISC-v Full Course https://youtube.com/playlist?list=PLqPfWwayuBvN1JkJFR9G1nQGXsNdi5aZ-&si=wWCQ9C7U0I_-T2cV
- Patterson, D. A., & Waterman, A. (2017). The RISC-V Reader: An Open Architecture Atlas. Strawberry Canyon LLC
- RISC-V Foundation. (2023). RISC-V Instruction Set Manual. https://riscv.org
- Hennessy, J. L., & Patterson, D. A. (2017). Computer Architecture: A Quantitative Approach. Morgan Kaufmann.

### License

This project is open-sourced under the MIT License. See the LICENSE file for more information.

 Contributions are welcome! Feel free to fork, enhance, and share your improvements to Custom RISC-V.

