# Fibonacci Sequence Generator for z/OS Unix

This project is a Fibonacci sequence generator written in assembly language, specifically tailored for z/OS Unix environments. It generates the first 40 results of the Fibonacci sequence and outputs them to stdout.

## Overview

- **Main Functionality:** Generates the first 40 numbers in the Fibonacci sequence.
- **Environment:** Designed for execution in z/OS Unix.
- **Output:** Utilizes BPX1WRT to print the results to stdout.

## Setup and Usage

### Prerequisites

- An environment running z/OS Unix.
- Access to assembly language compiler and linker for z/OS.

### Compilation and Execution

1. **Compile the Assembly Code:**
   - To compile the code, run the following command:
     ```
     as -o fibonacci.o fibonacci.s
     ```

2. **Link the Object File:**
   - Link the object file to create an executable:
     ```
     ld -o fibonacci fibonacci.o
     ```

3. **Run the Executable:**
   - Execute the program to see the Fibonacci sequence:
     ```
     ./fibonacci
     ```

4. **Output:**
   - Check the output in your terminal to see the first 40 numbers of the Fibonacci sequence.

## Components

- **Linkage and Getmain:** Sets up the necessary environment for the program, including obtaining storage.
- **Application Logic:** Contains the core logic for generating the Fibonacci sequence.
- **Subroutines:** Includes the TOSTDOUT subroutine for handling output to stdout.
- **Constants and Literal Pool:** Defines various constants and literals used in the program.

## File Structure

- `fibonacci.s`: The main assembly source file containing the program logic.
- `fibonacci.o`: The object file generated from the source file.
- `fibonacci`: The executable file generated from the object file.

## Acknowledgments

This project is an example of using assembly language for mathematical computations in a z/OS Unix environment. 

---

Feel free to explore and modify the code to suit your needs.
