# Chapter 1.1: Number Systems

Objectives

```
1. Understand the denary, binary and
hexadecimal number systems
2. Understand how and why computers use binary to represent all forms of data
3. Understand how and why hexadecimal is used as
a beneficial method of data representation
4. Convert

      binary ←→ denary
         ↑       ↑  
         ↓       ↓
        hexadecimal
        
5. Add two positive integer bytes
6. Perform logical binary shift on a positive byte
7. Use two's complement to represent positive and negative byte binary integers
8. Understand what is an overflow
```

## B-owerful binary

Computers use ``logic gates`` and ``registers`` to process and store data, which could only be in 2 states, ``an off and on state (aka 0 and 1)``. This defines the ``base-2 number system``, which we call binary.

Because computers are only able to process binary, ``any sort of data needs to be converted into binary for computers to process``. They also have a limited amount of size that its ``CPU (in Chapter 2)`` registers can store, such as 64-bit for most modern systems.

### Real-life note
```
Most x64 CPUs come with something called AVX registers, which can store 512 bits. However, this is not mentioned in the IGCSE syllabus (2023-2025), and therefore would not be useful in the real exam. Do not use this information.
```

## Hexadecimal

Is a base-16 number system (represented by 0-9 and A-F, e.g. 0xdeadbeef, 0xb0b, 0x123456789abcdef).

They are mostly used by software developers, specifically when programming in the ``assembly language``. ``Assemblers (in Chapter 4.2)``, also mostly use hexadecimal for representing ``opcodes and operands (in Chapter 4.2)``