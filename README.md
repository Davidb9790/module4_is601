Module 4 – Python Calculator Application (IS601)
Overview
   This project is a modular command‑line calculator built in Python.
   It supports addition, subtraction, multiplication, division, and power.
   The design uses clean architecture, a CalculationFactory, and full unit testing.

Supported Operations
   Addition
   Subtraction
   Multiplication
   Division
   Power (Exponentiation)

Project Structure
   Code
   app/
   │
   ├── calculation/
   │   └── __init__.py        # Abstract Calculation class, Factory, and operation classes
   │
   ├── operation/
   │   └── __init__.py        # Arithmetic logic for all operations
   │
   tests/
   │   ├── conftest.py        # Fixture to reset and re‑register calculations
   │   ├── test_calculation.py
   │   ├── test_operations.py
   │   ├── test_calculator.py
   │
   README.md
Calculation Classes
Each operation is implemented as its own class:
   AddCalculation
   SubtractCalculation
   MultiplyCalculation
   DivideCalculation
   PowerCalculation

Features
   REPL interface (continuous user input)
   Operations: add, subtract, multiply, divide, power
   Input validation
   Error handling (LBYL + EAFP)
   Calculation history
   Commands: help, history, exit
   Modular structure (operation, calculation, calculator)
   100% test coverage with pytest