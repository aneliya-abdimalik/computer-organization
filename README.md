# computer-organization
This repository contains four major labs that cover processor performance optimization, security exploits, binary reverse engineering, and pipeline architecture design.

## Technology Stack
- **Architecture:** x86-64 (Intel/AMD) and Y86-64 simulator
- **Languages:** C, x86-64 Assembly, Y86-64 Assembly
- **Tools:** GNU Make, gcc, gdb, objdump, hex2raw, Y86-64 simulators (YIS, SEQ, PIPE), Python scripts, Modelio/SysML
- **Libraries:** Standard C library, custom simulator libraries

## Labs Overview

1. **Performance Lab** (`perf_lab/`)
   - **Objective:** Optimize memory-intensive kernels (Normalization and Kronecker Product) for CPE reduction
   - **Description:** Implement and tune `normalize()` and `kronecker_product()` in `kernels.c`, measure cycles-per-element, and achieve speedups over naive versions 

2. **Attack Lab** (`attack_lab/`)
   - **Objective:** Develop code-injection and return-oriented programming (ROP) exploits against vulnerable binaries
   - **Description:** Craft exploit strings for `ctarget` (touch1–3 code-injection) and `rtarget` (ROP gadgets) to validate security vulnerabilities using `hex2raw` and GDB 

3. **Bomb Lab** (`bomb_lab/`)
   - **Objective:** Reverse-engineer and defuse multi-phase binary bombs under debugger control
   - **Description:** Disassemble and debug `bombk` executable across six phases, avoiding brute force and minimizing penalty on wrong guesses 

4. **Architecture Lab** (`arch_lab/`)
   - **Objective:** Extend and optimize pipelined Y86-64 processors and benchmark programs
   - **Description:** Part A: Write Y86-64 selection sort (iterative & recursive). Part B: Add `cmpq` to SEQ. Part C: Optimize `to_binary_string.ys` and PIPE control logic for performance 
