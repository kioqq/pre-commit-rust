# Rust hooks for pre-commit

[Rust](https://www.rust-lang.org) tools package for [pre-commit](https://pre-commit.com).

## Using rust tools with pre-commit

```yaml
- repo: https://github.com/kioqq/pre-commit-rust
  rev: v1.0
  hooks:
  - id: cargo-fmt
  - id: cargo-test
  - id: cargo-check
  - id: cargo-clippy
  # Take attention on notes section
  - id: cargo-audit
  - id: cargo-udeps
```

---
**NOTES**

* ```cargo-udeps``` needs the **nightly toolchain** and ```cargo-udeps``` installed (```cargo install cargo-udeps```)
* ```cargo-audit``` needs ```cargo-audit``` installed (```cargo install cargo-audit```)

---
