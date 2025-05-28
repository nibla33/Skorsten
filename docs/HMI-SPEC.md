# Skorsten HMI Specification

## Overview

The Skorsten HMI is a text-based graphical user interface layer for visualizing and interacting with `.sk` variables. It is designed to run in the terminal or lightweight embedded environments with minimal resources.

This interface mimics the clarity and structure of HTML/CSS but remains declarative, minimal, and purpose-built for automation.

---

## Core Design Goals

* Fully text-based and transparent
* Terminal-first display (ncurses, similar to TUI)
* Linked directly to `.sk` runtime variable state
* Modifiable via simple layout language (e.g., YAML, markup)
* Extendable for browser-based rendering later (HTML-like)

---

## MVP Features

* Define screens/views in `.hmi` files
* Bind live `.sk` variables to elements
* Display variable states (boolean, integer, float, strings)
* Simple layout blocks:

  * Labels
  * Buttons (future interactivity)
  * Indicators (on/off)
* Refreshable interface synced with runtime state
* Standalone CLI (`skhmi`) to run in terminal

---

## Syntax Example

```hmi
screen Main {
  label: "Tank Level"
  value: tank.level

  label: "Valve Status"
  indicator: valve.open
}
```

---

## Future Extensions

* Layout control (columns, grids, tabs)
* Input controls: buttons, sliders (with linked `.sk` variables)
* Network interface: remote HMI over SSH or HTTP
* Plugins to render in browsers
* Theme support (colors, visual config)

---

## Long-Term Vision

* Full separation of logic (PLC) and interface (HMI)
* Developer-first: easy to edit, version, and deploy
* HMI marketplace with themes, prebuilt blocks, and visual editors
* Ideal for remote, headless, or containerized systems

---

## Out of Scope

* Native touchscreen support (optional plugin)
* Complex SCADA-level visualization (not a goal)
* Binary HMI formats or closed tooling
