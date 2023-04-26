 # Authors of RISC CPU

# Engineers
* Justin Koe
* Diego Toribio

# Artifacts

## Instruction Set Architecture (ISA)
< This ISA is based off the RISC-V ISA (RV32I) with the main changes being made to register usage rather than actual instruction format >
* Justin Koe (50%)
* Diego Toribio (50%)

## CPU Implementation in Verilog

### Instruction Memory/Data Memory
* Justin Koe (100%)
    * Wrote test programs
    * Made easy way to load instructions into instruction memory: implemented $readmemb() function
    * Created data memory

### Register File
* Diego Toribio (100%)
    * Created registers to load input values and store the results from operations

### ALU
* Justin Koe (100%)
    * Incorporated all planned operations into Verilog

### Controller/Control Path
* Justin Koe (100%)
    * Created the main control unit and ALU control unit
    * Derived control lines from opcode
    * Created instruction decoder
    * Created immediate value decoder

### Program Counter 
* Diego Toribio (100%)
    * Created PC modules
        * PC_adder: increments PC by 4 at every positive edge
        * Jump_adder: adds immediate from instruction to PC if branching
        * PC_mux: decide which PC is used for the following instruction

### Datapath
* Justin Koe (80%)
    * Created modules that operate on data, store and read data from memory, and control data writeback
* Diego Toribio (20%)
    * Created module that controlled second input of ALU 

### Verilog Test Bench for Computer
* Justin Koe (100%)
    * Pulled together all modules in the cpu_tb.v to test CPU

## Compilation of Assembly Code into Machine Code
* Justin Koe (75%)
    * Wrote Test_Program.txt and compiled to machine code
    * Wrote Fibonacci_Sequence.txt 

* Diego Toribio (25%)
    * Compiled Fibonacci_Sequence.txt into machine code

## Timing Diagrams

### R-Type Instruction example
* Diego Toribio (100%)
    * Ran Test_Program.txt and analyzed the R-type instructions

### I-Type Instruction example
* Justin Koe (100%)
    * Ran Test_Program.txt and analyzed the I-type instructions

### B-Type Instruction example
* Diego Toribio (100%)
    * Ran Test_Program.txt and analyzed the B-type instructions

### S-Type Instruction example
* Justin Koe (100%)
    * Ran Test_Program.txt and analyzed the S-type instructions

### Fibonacci Sequence example
* Justin Koe (100%)
    * Ran Fibonacci_Sequence.txt and analyzed the signals to ensure the Fibonacci sequence was generated