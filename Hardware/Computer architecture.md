# Chapter 3.1: Computer architecture

Objectives
```
Understand what is a microprocessor, and the Von Neumann architecture and their purpose
Understand the purpose of a CPU
Understand what is meant by a core, cache and clock of a CPU
Describe the purpose and characteristics of an embedded system and identify them on commonly used devices.
```

## Big computer brain

In a computer, the CPU is the one which ``processes instructions and data that are input`` into the
computer so that the ``result can be output``. Many modern CPUs follow the Von Neumann architecture,
which consists of a single, shared memory for programs and data, a single bus for memory access, 
an arithmetic unit, and a program control unit. It's based on the principle of the FDE cycle.

A diagram is shown below

![An image of the Von Neumann architecture in a CPU](https://media.geeksforgeeks.org/wp-content/uploads/basic_structure.png)

Units:
* Arithmetic Logic Unit (ALU) is the unit which performs bitwise (logical) operations and arithmetic operations.
* Control Unit (CU) is the unit that sends signals to coordinate how data move around the CPU, and decodes instructions fetched from memory

Buses:
* Control bus is a bidirectional bus that carries commands and control signals to tell components when should they read or write
* Data bus is a bidirectional bus that carries data or instructions
* Address bus is a unidirectional that carries addresses

Registers:
* Program Counter (PC) is a register that holds the next address of the next instruction to be executed
* Memory Address Register (MAR) is a register that holds the memory address of where data or instructions are to be fetched from memory
* Memory Data Register (MDR) is a register that stores the data or instruction
* Current Instruction Register (CIR) is a register that stores the instruction the CPU is decoding and executing
* Accumulator (ACC) stores the result of operations performed by the ALU

## Fetch, decode and execute

The FDE (fetch-decode-execute) cycle is the principal on which the Von Neumann architecture is based on.

It states that the CPU executes code by,

### Fetching
the instruction in memory by the address stored in the Memory Address Register (MAR), which was at first stored in the Program Counter (PC), and storing the read instruction, signaled by the control unit, into the Memory Data Register (MDR)

### Decoding
the instruction is then copied from the Memory Data Register (MDR) to the Current Instruction Register (CIR) and decoded by the control unit

### Executing
the control unit then executes the instructions accordingly, and the address in the Program Counter (PC) is incremented by 1

## CPU

There are a variety of CPU manufactuerers in the world. AMD and Intel both produce x64 and x86 (not anymore because its redundant for modern use) CPUs, and finally, Qualcomm and NVIDIA for ARM and RISC-V CPUs.

What sets the difference between the CPUs, however, are their instruction sets. Intel's x64 CPUs might have a slight difference in instructions compared to AMD's x64 CPUs, depending on the model. It basically dictates how much a CPU can do.

There are also other differences, too. The number of cores, for example may also differ between CPU models. A core is what we were refering to as a "CPU". They contain the units, buses and the registers. If a CPU model has 2 cores, it means that the CPU can execute twice as many instructions as compared to a single core CPU.