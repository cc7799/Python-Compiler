# Python to x86 Compiler
A simple python to x86 compiler that supports features such as varibles, tuples, functions, garbage collection, and 
  more.

This was created as a course project for the Compiler Construction (CS 3020) course I took as a student at UVM.

## Table of Contents
* [Description](#description)
* [Installation & Setup](#installation--setup)
  * [Prerequisites](#prerequisites)
  * [Setup](#setup)
* [Operation](#operation)
* [Code Authorship](#code-authorship)


## Description
This compiler compiles standard python code to x86. It has some restrictions compared to a standard python compiler, 
  but does support many features.
Several tests designed to demonstrate the features of the compiler are included in the `tests` folder.

<u>Features</u>
1. Booleans
2. Integers
3. Tuples
4. Arithmetic
5. Variables
6. If-statements
7. While loops
8. Functions (including recursion)
9. Efficient register and memory allocation
10. Garbage collection

<u>Major Restrictions</u>
1. The compiler does not support strings or any non-integer numbers
2. The compiler does not support for-loops
3. The compiler is statically-typed and does not support dynamic typing
4. Variables and parameters must be declared with type-annotations
5. Functions must have return type-annotations

## Installation & Setup
### Prerequisites
The project requires the `lark` and `pandas` libraries which can be installed using `pip`.
Python 3.10 or higher is also required due to the use of match statements.

The project uses a slightly modified version of a python parser provided by the course professor. 
The original code can be found [here](https://github.com/jnear/cs202-assignments/tree/main/cs202_support).
The modified code is in the `parser` and `program_lang` folders.

### Setup
No setup beyond installing the prerequisites is required.

## Operation
The code is run by running the `run_tests.py` script.
This compiles every file in the `tests` folder. 
It runs the compiled code and runs the original code through an interpreter.
The results are then printed and compared.

## Code Authorship
The compiler passes found in `compiler.py`, which make up the majority of the code-base were written by me.
The tests in the `tests` folder were also written by me.

The support code was provided by the course professor. 
This includes, All code in the `parser` and `program_lang` folders apart from some minor changes, 
  and all code in the main folder other than `compiler.py`.

