# Skorsten — Open Source PLC Runtime & Text-Based HMI for a New Era

**Status:** Pre-MVP — Groundwork phase
**Author:** Albin Magnusson
**License:** MIT

---

## 🌍 Vision

**Skorsten** is a modular, open-source automation platform that rethinks how PLC systems and HMI interfaces are designed and developed.

It consists of two tightly related but technically distinct components:

1. **Skorsten Runtime** – A Linux-native PLC runtime written in Rust, using a custom plaintext control language (`.sk`)
2. **Skorsten HMI** – A lightweight, text-declarative HMI layer, inspired by HTML/CSS but built specifically for automation

Together, they offer a minimal, extensible, and fully transparent foundation for modern industrial control — focused on Linux, real-time behavior, and developer-first workflows.

---

## ✨ Core Principles

* 📄 **Plaintext by Default** — No binary formats or hidden logic; everything version-controllable
* 🪶 **Modular and Minimal** — Base install is tiny; every feature is opt-in via plugins or modules
* 🧰 **Hackable & Transparent** — No lock-in, no secrets, fully inspectable
* 💻 **Linux-First** — Designed from the start for edge devices and embedded Linux
* 🌱 **Sustainable and Extensible** — Plugins and modules can be community-made or commercial
* 🧠 **Built for Developers** — Testing, simulation, AI tooling, and structured collaboration are priorities

---

## 🤔 Why Skorsten?

The industrial automation world is filled with legacy systems:

* Closed, monolithic software stacks
* Windows-only vendor tools
* Poor support for modern dev workflows
* Expensive, non-portable HMI systems

Skorsten is your clean break from all that.

---

## 🧱 Project Scope

### 🔧 Skorsten Runtime (PLC Core)

* `.sk` files define automation logic in an extended structured text dialect
* Rust-based runtime on Linux executes control loops
* Targeted at small form-factor PCs and SBCs like the Raspberry Pi

### 🗅 Skorsten HMI

* HMI definitions written in plaintext using a declarative syntax
* Rendered as a live UI in a terminal or minimal GUI backend
* Meant for embedded use, browser rendering optional later

> The HMI and PLC are designed to function independently but integrate tightly.

---

## 🚧 Roadmap

The development plan is split into components and chronological phases. View the full [roadmap here](./ROADMAP.md).

---

## 📖 Linked Docs

* [ROADMAP.md](./ROADMAP.md) — Full project development roadmap
* [docs/SK-LANGUAGE.md](./docs/SK-LANGUAGE.md) — `.sk` language design and syntax
* [docs/HMI-SPEC.md](./docs/HMI-SPEC.md) — Text-based HMI specification

---

## 🧰 Contributing

Skorsten is currently in its groundwork phase and **not yet open for contributions**. Once the foundations are stable, guidelines and issues will be posted.

---

## 🛠 Tech Stack

* **Runtime Language:** Rust
* **Target Platform:** Linux (RT kernel optional)
* **Logic Format:** `.sk` (structured text dialect)
* **HMI Format:** `.hmi` (plaintext markup, WIP)

---

## 📨 Contact

**Albin Magnusson** – Creator of Skorsten
📧 Email: [albin.magnu@gmail.com](mailto:albin.magnu@gmail.com)
🖥 GitHub: [github.com/YOURUSERNAME](https://github.com/YOURUSERNAME)

---

> *“Skorsten is a rejection of industrial software bloat — it's a toolbox for engineers who want control, clarity, and creativity in automation.”*
