# Day 1 : FPGA Introduction
This is a take of an FPGA Prototyping Tool Verification Engineer from the workshop.
## FPGA Architecture
An FPGA mainly consists of:
- Configurable Logic Blocks (CLBs): The combinational logic block (CLB) is a fundamental building block in FPGAs that implements logic functions without memory. CLBs are organized in an array across the FPGA fabric.The CLB operates by receiving inputs from connected signals, using the LUT as a lookup table to map input combinations to outputs, producing output based on the programmed truth table and routing the output through multiplexers to other CLBs or I/O blocks. Flip Flops are used for Sequential Logic and Carry chains are used for arithmetic operations.
- Look-Up Tables (LUTs): The core component of every CLB is the Look-Up Table (LUT). LUTs are typically 4-input, 5-input, or 6-input configurations, depending on the FPGA architecture. These LUTs function as a small RAM that stores truth tables for logic functions. The primary advantage of LUTs is that they can implement any Boolean function of their input variables, making them extremely versatile. For example, a 4-input LUT can represent any logic function of 4 variables, allowing designers to program custom logic functions directly into the FPGA without being limited to predefined gate types. This programmability is what enables the flexibility and power of FPGA-based digital design.
- Flip-Flops (FFs): Following is the role of Flip-Flops in FPGA.
  1. Sequential Logic Implementation: Enable construction of finite state machines, counters, and shift registers
  2. Data Storage: Provide single-bit memory elements for storing data across multiple clock cycles
  3. Clock Synchronization: Capture and align data with clock edges to prevent timing violations
  4. CLB Integration: Co-located with LUTs in logic cells, allowing programmable registered or combinational outputs
  5. Pipeline Architecture: Break long combinational paths into stages to increase maximum clock frequency
  6. I/O Buffering: Synchronize external signals with internal clock domains at FPGA interfaces
  7. Metastability Prevention: Mitigate timing issues in asynchronous clock domain crossings
  8. Timing Closure: Reduce critical path delay and ensure setup/hold time compliance
- Programmable Interconnects
- Block RAM
- DSP Blocks
- I/O Blocks
- Clock Tiles: 

