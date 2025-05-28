# Skorsten Project Roadmap

> This roadmap is subject to change as development progresses and feedback is gathered. All dates are approximate and depend on available development time.

---

## Phase 0: Groundwork (Now)

**Goal:** Establish foundation for runtime, language, and tooling.

* [x] Define project philosophy and scope
* [x] Set up Git repository and initial structure
* [x] Define modular architecture approach
* [x] Draft initial README and documentation layout
* [ ] Begin Rust runtime scaffold
* [ ] Define initial `.sk` language syntax and parser design

---

## Phase 1: PLC Runtime MVP

**Goal:** Basic `.sk` program execution with internal simulation loop

* [ ] Implement minimal Rust runtime

  * Parse `.sk` files with variable declarations
  * Execute basic scan loop with cycle timing
  * Track and print variable states
* [ ] CLI runner tool (`skrun`) for executing `.sk` programs
* [ ] Add support for timers, simple IF/WHILE logic
* [ ] Logging and debug output
* [ ] Write unit tests for runtime components

---

## Phase 2: HMI MVP (Text-based Interface)

**Goal:** Terminal-based HMI renderer with live variable bindings

* [ ] Define `.hmi` syntax (markup-like)
* [ ] Basic terminal renderer with live updates
* [ ] Bind variables to displays
* [ ] Optional config layout (YAML or inline)
* [ ] Build standalone CLI (`skhmi`) to view HMI

---

## Phase 3: IO & Communication

**Goal:** Support basic IO modules and mock drivers

* [ ] GPIO and mock IO backends
* [ ] Real-time IO polling interface
* [ ] Add IO mapping to `.sk` programs
* [ ] Early OPC UA client integration (optional plugin)
* [ ] Simulated devices for development without hardware

---

## Phase 4: Language Expansion & Developer Tooling

**Goal:** Extend `.sk` language and provide automation-friendly features

* [ ] Add functions, function blocks, and classes
* [ ] OOP features: inheritance, interfaces
* [ ] Dynamic vectors and memory safety
* [ ] Type checking and compile-time validation
* [ ] Online/monitor mode: inspect and force variables
* [ ] Implement test framework for `.sk` logic

---

## Phase 5: Community & Ecosystem

**Goal:** Open contributions, documentation, and collaboration tools

* [ ] Documentation portal (mkdocs or similar)
* [ ] Tutorials and example projects
* [ ] Contributor guides and issue templates
* [ ] Launch Discord/Matrix or forum space
* [ ] Accept limited pull requests

---

## Phase 6: Marketplace & Plugin Model (Separate Project)

**Goal:** Launch commercial ecosystem without compromising openness

* [ ] Define plugin API/spec for Skorsten extensions
* [ ] Build simple marketplace for:

  * Custom modules (e.g. Profinet drivers)
  * Hardware integrations
  * Premium HMIs or testing tools
* [ ] Provide SDK and CLI tools to develop/distribute plugins
* [ ] Optional vendor-backed bundles or hardware kits

---

Want to contribute? Not yet — groundwork is still being laid. Stay tuned!
