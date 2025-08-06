## Custom RISC-V Processor

![RISC-V]<img width="313" height="161" alt="download" src="https://github.com/user-attachments/assets/f30d9dac-f40f-4ec5-9ea3-f86d7bd4c7d7" />

VEGA Core is a custom-designed 32-bit RISC-V processor developed using Verilog HDL. Built from the ground up as part of an educational and research-focused initiative, it supports the RV32I base instruction set and features a clean, modular, and pipelined architecture. This project is ideal for students, researchers, and hobbyists interested in processor design, computer architecture, and FPGA prototyping.

### Features

- Fully functional RV32I base instruction set support
- Designed using Verilog HDL with clean modular hierarchy
- Includes all essential components:
  - Instruction Fetch Unit
  - Decoder / Control Unit
  - Register File
  - ALU (Arithmetic Logic Unit)
  - Branch Control Logic
  - Data Memory
- Implements 5-stage pipelining: IF, ID, EX, MEM, WB
- Verified through module-level and system-level testbenches
- Synthesizable and deployable on FPGA (target: PYNQ-Z2)
- Compatible with GTKWave for waveform analysis


### Simulation & Verification

- Run simulations using Icarus Verilog or ModelSim.
- Use GTKWave to view waveform outputs.
- Testbenches include instruction sequences and corner cases.

### Example (using Icarus Verilog):

iverilog -o cpu_tb tb/cpu_tb.v rtl/*.v
vvp cpu_tb
gtkwave dump.vcd

### FPGA Deployment (PYNQ-Z2)

- Synthesis flow supported via Open-source tools
- Constraint file included for PYNQ-Z2 pin mapping
- Load program memory with instruction hex files
- UART/LEDs can be used to observe processor output

### Project Goals

Custom RISC-V is developed to:
- Educate learners on real-world CPU architecture and design
- Provide a foundation for experimenting with custom ISAs
- Explore extensions such as RV32M, caching, hazard detection, forwarding, etc.
- Enable hands-on prototyping using affordable FPGA platforms

### References

- RISC-V Official Specs: https://riscv.org/specifications/
- FPGA: PYNQ-Z2 Board: https://www.tul.com.tw/ProductsPYNQ-Z2.html

### License

This project is open-sourced under the MIT License. See the LICENSE file for more information.

 Contributions are welcome! Feel free to fork, enhance, and share your improvements to Custom RISC-V.

