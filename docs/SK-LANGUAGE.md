# Skorsten PLC Runtime Scope

## Overview

The Skorsten PLC runtime is a Linux-native, Rust-based execution engine for a modern structured text dialect (`.sk`). It is designed to be:

* Fully modular and minimal at its core
* Deterministic and cycle-based
* Transparent and Git-friendly (all plaintext)

This document outlines the core scope and priorities of the runtime portion of the Skorsten project.

---

## Runtime Core Features (MVP)

* Minimal parser for `.sk` syntax (Rust-based)
* Internal data representation and memory handling
* Main loop with cycle timing (scan, compute, update)
* Variable definition and runtime tracking
* Logging, error output, debug mode
* CLI to run `.sk` files and view output

---

## Language Features (Initial)

* Variable declarations (with types and initial values)
* Simple expressions and operations
* Control flow: `IF`, `WHILE`, `CASE`
* Timers and counters (basic function blocks)
* Structured organization into function blocks

---

## Planned Extensions (Post-MVP)

* Object-oriented features:

  * Classes with inheritance and interfaces
  * Dynamic vectors, user-defined types
* Online monitoring and forcing of variable values
* External IO abstraction and mapping
* Test harness for logic validation
* Compilation to bytecode/intermediate form (optional)

---

## Long-Term Scope

* Plugin support for industrial protocols (e.g., Modbus, OPC UA)
* Integration with HMI interface and live debugging
* Target multiple hardware platforms (ARM, x86)
* Real-time kernel compatibility
* Safety features and failover modes (future optional modules)

---

## Out of Scope

* Web IDE (leave to third-party tools)
* Proprietary protocol stacks
* Legacy compatibility (e.g., IEC61131-3 certification)
