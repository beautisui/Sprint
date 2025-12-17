# Sprint - A Low-Level Programming Language

## Overview
Sprint is a **low-level assembly-like language** designed to help understand how computers work at a fundamental level. It's a simplified programming environment where you work with memory addresses, pointers, and basic operations to build logic.

## What is Sprint?

Sprint teaches you how programs actually work "under the hood" by eliminating abstractions. Instead of writing `result = a + b`, you:
- Load values from memory addresses
- Perform operations
- Store results back to memory
- Jump between instructions

This hands-on approach helps you understand:
- Memory management
- Program flow control
- How high-level operations break down into basic steps

## Core Concepts

### Memory & Pointers
- **Addresses**: Locations in memory where data is stored
- **Pointers**: Variables that hold memory addresses
- **Values**: The actual data stored at an address

### Program Structure
```
instruction_name:operation_code param1 param2 ...
```

- **Operation codes** (0-10) define what to do
- **Parameters** are addresses or pointers to data

## Available Operations

| Code | Name | Purpose |
|------|------|---------|
| 0 | `put` | Store a value at a memory address |
| 1 | `load` | Load a value from an address |
| 2 | `increment` | Increase a value by 1 |
| 3 | `jump` | Jump to another instruction |
| 4 | `jump_if_equal` | Jump if two values are equal |
| 5 | `jump_if_less` | Jump if one value is less than another |
| 7 | `copy` | Copy value from one address to another |
| 9 | `stop` | End the program |
| 10 | `multiplication` | Multiply two numbers |

## Built-in Arithmetic Operations

### `addition`
Adds two numbers and stores the result
- Takes 3 parameters: address of first number, second number, result address

### `subtraction`
Subtracts one number from another
- Takes 3 parameters: address of first number, second number, result address

### `multiplication`
Multiplies two numbers using loops
- Takes 3 parameters: address of first number, second number, result address

### `copy`
Copies a value from one memory address to another
- Takes 2 parameters: source address, destination address

## How a Sprint Program Works

1. **Initialization**: Set up pointers and initial values
2. **Execution**: Follow instructions step by step
3. **Jumps**: Change program flow based on conditions
4. **Loops**: Jump back to repeat operations (for counting, iterating)
5. **Termination**: Stop when done

## Example Concepts

### Loop Pattern
```
operation:instruction to perform
jump_back:jump to operation label
```
This creates a loop by jumping back to a previous instruction.

### Conditional Jump
```
check_value:jump_if_equal value1 value2 next_step
```
If two values match, continue; otherwise, jump to next_step.

## Getting Started

1. Understand the **memory model** - everything is stored at an address
2. Learn the **operation codes** - what each number (0-10) means
3. Trace through **one operation** - see how values move through memory
4. Build **simple arithmetic** - use addition/subtraction first
5. Add **control flow** - learn jumps and loops
6. Create **complex programs** - combine operations

## Key Takeaways

✓ Every program is a sequence of memory operations  
✓ All computation breaks down into load, calculate, store  
✓ Control flow (jumps) makes programs interactive  
✓ Loops are created by jumping backwards  
✓ Conditions allow dynamic program behavior  

## Learning Value

By writing in Sprint, you'll understand:
- Why computers need RAM and how it works
- How assembly language functions
- The relationship between high-level code and machine operations
- Why pointers are fundamental to programming
- How programs actually execute step-by-step

---

**Sprint**: Learn programming from the ground up! 🚀
