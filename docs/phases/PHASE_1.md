# Phase 1: Basic Language Parsing and Runtime Prototype

## Overview

The primary objective of Phase 1 is to develop a minimal but functional subset of the ST (Structured Text) language tailored for our `.sk` dialect. This phase will focus on:

- Defining core language features such as basic data types, variable declarations, and fundamental control flow.
- Implementing a parser that translates `.sk` code into Rust.
- Creating a simple runtime capable of setting variables and executing basic logic.

This phase also serves as an opportunity to improve Rust skills and adopt Test-Driven Development (TDD) practices. All code and documentation will be maintained openly on GitHub to encourage transparency.

---

## Language Dialect Scope for Phase 1

The following features will be supported initially:

### Data Types

- `INT` (mapped to Rust `i32`)
- `BOOL` (mapped to Rust `bool`)
- `REAL` (mapped to Rust `f32` or `f64`)

### Variable Declaration

```sk
VAR
  counter : INT;
  flag : BOOL;
END_VAR
````

* Variables can be declared within a `VAR...END_VAR` block.
* All variables are mutable by default.

### Assignments

```sk
counter := 10;
flag := TRUE;
```

* Simple assignment statements using `:=`.

### Control Flow

* `IF...THEN...ELSE` statements

```sk
IF counter > 0 THEN
  flag := TRUE;
ELSE
  flag := FALSE;
END_IF
```

* `CASE` statements for multi-branch logic

```sk
CASE counter OF
  0: flag := FALSE;
  1: flag := TRUE;
ELSE
  flag := FALSE;
END_CASE
```

* `WHILE` loops (optional, based on time/resources)

```sk
WHILE counter < 10 DO
  counter := counter + 1;
END_WHILE
```

### Limitations

* No functions, function blocks, or classes in this phase.
* No external IO or hardware interaction.
* Focus on internal logic and simulation only.

---

## Technical Details

### Parsing

* Use Rust parser libraries (`nom` or `pest`) to build a parser for `.sk` syntax.
* Convert parsed input into an Abstract Syntax Tree (AST) representation.
* Translate AST into Rust code that simulates PLC scan cycle logic.

### Runtime

* Rust executable that:

  * Declares and initializes variables.
  * Executes a simulated scan loop (initially just one iteration).
  * Applies the parsed logic (assignments, control flow).
  * Prints variable states to the terminal on each cycle.

### CLI Tool

* Develop a command-line tool (`skrun`) to:

  * Load `.sk` files.
  * Parse and compile to Rust code.
  * Run the generated Rust code or run it via a Rust interpreter (as implemented).

---

## Testing and Debugging

* Use terminal output for immediate feedback on variable states and logic execution.
* Print detailed logs for each step of the scan cycle.
* Implement unit tests for parsing, AST generation, and runtime components.
* Adopt Test-Driven Development (TDD) for critical parts of the parser and runtime.
* Keep tests and examples alongside source code for easy verification.

---

## Goals Summary

By the end of Phase 1, we expect to have:

* A working `.sk` parser that covers basic variable declarations, assignments, and control flow.
* A Rust runtime skeleton capable of executing parsed `.sk` logic in a simulated PLC scan loop.
* A CLI tool to run and debug `.sk` programs with console output.
* Documentation and tests covering the implemented features.

---

*This document will evolve as development progresses. Community feedback and contributions will be welcomed once the foundation is stable.*

```
