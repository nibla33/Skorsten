# Skorsten — Modern, Open PLC Runtime & Text-based HMI

**Status:** Early MVP — actively in development

---

## Vision

Skorsten is a minimalist, modular, open-source PLC runtime and HMI platform designed for mechatronics engineers and hardware hackers who want:

- Full control over their automation code with plaintext, Git-friendly files
- A modern, Linux-native toolchain free from vendor lock-in
- Developer-first experience with AI, automation, and testing in mind
- A text-based HMI interface designed for terminal and lightweight devices

Our mission is to transform industrial automation tooling by bringing it into the 21st century.

---

## Why Skorsten?

Existing PLC solutions are often:

- Closed and proprietary, locking you into expensive ecosystems
- Windows-only and not friendly to modern development workflows
- Difficult to version control and collaborate on
- Poorly suited to automation, AI-assisted development, or embedded Linux

Skorsten aims to fix these issues by being:

- Open and modular, with a plugin-friendly architecture
- Text-based with all files in plaintext, perfect for Git and CI/CD
- Lightweight and Linux-first, optimized for SBCs and edge devices
- Focused on developer productivity and future-proof automation

---

## Roadmap

### Phase 1: Foundation (Initial MVP)
- Build a minimal runtime capable of parsing variables and executing a basic loop
- Implement a simple text-based HMI that displays live variable states in the terminal
- Create a CLI tool to run `.sk` programs on Linux
- Develop minimal example `.sk` programs and documentation
- Target: Initial MVP ready within a few months, progress depending on available time

### Phase 2: IO & Simulation (Ongoing Development)
- Add support for real and simulated IO drivers (e.g., GPIO, mock signals)
- Improve the HMI with configurable layouts using a simple DSL or YAML
- Introduce a unit testing framework for `.sk` logic
- Publish example projects demonstrating hardware integration
- Timeline: Rolling improvements as time permits, community contributions encouraged

### Phase 3: Extensions & Community Building
- Extend the language with control flow constructs (`IF`, `WHILE`, functions)
- Add support for user-defined types and OOP-like features in `.sk`
- Create thorough documentation, tutorials, and contributor guides
- Foster a growing community via GitHub, forums, or chat platforms
- Timeline: Iterative growth alongside user feedback and contributions

### Phase 4: Release & Monetization (Long Term Vision)
- Provide prebuilt Linux packages and easy installer scripts
- Establish an official website and expand social media presence
- Explore revenue models: support contracts, premium features, hardware bundles
- Develop a browser-based HMI and remote monitoring capabilities
- Timeline: Longer term goals, dependent on project traction and resources

---

## Getting Started

1. Clone the repo
2. Write `.sk` programs in plaintext Structured Text dialect
3. Run programs using the CLI runtime (`cargo run -- program.sk`)
4. Watch your variable states update in the terminal-based HMI

---

## How to Contribute

Contributions are welcome! Please open issues or pull requests for:

- Bug fixes
- Feature suggestions
- Documentation improvements
- Example projects

---

## License

MIT License — 

---

## Contact

Albin Magnusson — creator of Skorsten  
Email: albin.magnu@gmail.com  

