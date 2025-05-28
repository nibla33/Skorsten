# Rust Getting Started Guide for Skorsten

This document outlines the beginner-friendly steps and resources for learning Rust and starting development on the Skorsten Phase 1 runtime.

---

## 1. Get Comfortable with Rust Basics

- **Install Rust:** Follow the official guide at [rustup.rs](https://rustup.rs/)  
- **Learn Rust fundamentals:**  
  - The Rust Programming Language (The official book): https://doc.rust-lang.org/book/  
  - Rust by Example: https://doc.rust-lang.org/rust-by-example/  
  - Practice exercises on [Exercism Rust track](https://exercism.io/tracks/rust) or [LeetCode](https://leetcode.com/problemset/all/) (filter for easy problems)  

Focus especially on:  
- Variables and mutability  
- Functions and control flow (`if`, `match`, loops)  
- Ownership and borrowing concepts  
- Structs and enums basics  

---

## 2. Explore Cargo and Project Structure

- Learn how Cargo works — Rust’s package manager and build tool.  
- Create a sample Rust project (`cargo new my_project`) and understand the folder layout.  
- Practice compiling and running programs using `cargo run`.

---

## 3. Understand Parsing Basics

- Research parser combinators and libraries like [`nom`](https://github.com/Geal/nom) or [`pest`](https://pest.rs/).  
- Start building simple parsers for tiny inputs, such as `x := 10;`.  
- Follow tutorials on using `nom` or `pest` for parsing.

---

## 4. Build a Minimal Parser for `.sk` Variables

- Begin with parsing simple variable declarations, e.g.:

  ```sk
  VAR
    counter : INT;
  END_VAR
````

* Define Rust structs to represent these variables in your Abstract Syntax Tree (AST).
* Write unit tests to ensure your parser works correctly.

---

## 5. Simulate Runtime Logic

* Create Rust code structures to store variable states in memory (like using a `HashMap` or structs).
* Implement a simple scan loop that updates or prints variables to the terminal.
* Gradually add parsing and execution support for assignments and control flow (`IF` statements).

---

## 6. Incremental Test-Driven Development (TDD)

* Write tests for each new feature or component before or alongside implementation.
* Use Rust’s built-in testing framework (`cargo test`).
* Keep tests small, isolated, and easy to maintain.

---

## 7. Document Your Journey

* Keep notes on learning progress and design decisions.
* Update your GitHub repository regularly with progress and future plans.

---

## Helpful Tips

* Break problems into small, manageable parts; don’t try to solve everything at once.
* Use the Rust Playground ([https://play.rust-lang.org/](https://play.rust-lang.org/)) for quick experiments.
* Join Rust communities for support: [Rust Users Forum](https://users.rust-lang.org/) or Stack Overflow.
* Look at existing open source Rust projects related to parsing and CLI tools for inspiration.

---

If you need help getting started with Rust code or setting up the project structure, feel free to ask!

```

---

Would you like me to help you set up a minimal Rust project template for this too?
```
