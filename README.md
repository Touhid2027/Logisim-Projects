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
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

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

