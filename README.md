# 7-Segment Display Using K-Map

This project demonstrates how to design a 7-segment display decoder using Karnaugh Maps (K-Maps). The logic implementation is done using Basic Gates, NAND, NOR, SOP (Sum of Products), and POS (Product of Sums).

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [How It Works](#how-it-works)
- [Components](#components)
- [Circuit Design](#circuit-design)
  - [K-Map Simplifications](#k-map-simplifications)
  - [Logic Implementations](#logic-implementations)
    - [Basic Gates](#basic-gates)
    - [NAND](#nand)
    - [NOR](#nor)
    - [SOP](#sop)
    - [POS](#pos)

## Introduction

A 7-segment display is commonly used in digital electronics to represent numbers and some alphabets. This project focuses on implementing a logic circuit for a 7-segment display using K-Map-based simplifications.

## Features
- Implements logic for all 7 segments: a, b, c, d, e, f, g.
- Provides K-Map-based simplifications for each segment.
- Multiple implementation methods: Basic Gates, NAND, NOR, SOP, and POS.

## Components
- **Input Variables:** 3 binary inputs (A, B, C).
- **Output Segments:** 7 outputs (a, b, c, d, e, f, g).
- **Logic Gates:** AND, OR, NOT, NAND, NOR.

## Circuit Design

### K-Map Simplifications

Each segment (a-g) has a truth table that maps input combinations to output values. Using K-Maps, these truth tables are simplified into minimal logical expressions.

### Logic Implementations

#### Basic Gates
- Simplified Boolean expressions are implemented directly using AND, OR, and NOT gates.

#### NAND
- All logic is implemented using only NAND gates by transforming the Boolean expressions.

#### NOR
- All logic is implemented using only NOR gates by transforming the Boolean expressions.

#### SOP (Sum of Products)
- The minimized SOP form of the Boolean expressions is used to implement the logic.

#### POS (Product of Sums)
- The minimized POS form of the Boolean expressions is used to implement the logic.

# 32-Bit CPU Design

This project showcases the design and implementation of a 32-bit CPU. The CPU includes a 32-bit ALU (Arithmetic Logic Unit), a 32-bit Register File, Instruction Memory, and a fully completed 32-bit datapath.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Architecture Overview](#architecture-overview)
- [Components](#components)
  - [32-Bit ALU](#32-bit-alu)
  - [32-Bit Register File](#32-bit-register-file)
  - [Instruction Memory](#instruction-memory)
  - [32-Bit Datapath](#32-bit-datapath)
- [How It Works](#how-it-works)

## Introduction

This project aims to design a simple but functional 32-bit CPU capable of executing basic instructions. The CPU is built to demonstrate concepts of computer architecture and digital design.

## Features
- **32-bit ALU:** Supports arithmetic and logical operations.
- **32-bit Register File:** Contains general-purpose registers for temporary data storage.
- **Instruction Memory:** Stores the program to be executed.
- **Completed 32-bit Datapath:** Ensures seamless execution of instructions, including fetch, decode, execute, memory access, and write-back stages.
- Modular and scalable design.

## Architecture Overview

The CPU follows a single-cycle architecture, where each instruction is executed in a single clock cycle. It includes the following stages:
1. **Instruction Fetch:** Fetch the instruction from the instruction memory.
2. **Instruction Decode:** Decode the instruction and read necessary registers.
3. **Execution:** Perform operations using the ALU.
4. **Memory Access:** Access data memory (if required).
5. **Write Back:** Write results back to the register file.

## Components

### 32-Bit ALU
- Performs arithmetic (addition, subtraction) and logical (AND, OR) operations.

### 32-Bit Register File
- Contains a set of 32 general-purpose registers.
- Allows two read operations and one write operation per cycle.

### Instruction Memory
- Stores the machine code of the program.
- Provides a 32-bit instruction for each clock cycle.

### 32-Bit Datapath
- Combines the ALU, Register File, Instruction Memory, and Control Unit(Not Implemented Yet).
- Implements the complete instruction execution process.

## How It Works

1. **Fetch:** The Program Counter (PC) fetches the next instruction from Instruction Memory.
2. **Decode:** The Control Unit decodes the instruction and generates control signals for the datapath(This is done manually for now).
3. **Execute:** The ALU performs the required operation as specified by the instruction.
4. **Memory Access:** Data is read from or written to memory if the instruction requires.
5. **Write Back:** The result is written back to the Register File.

