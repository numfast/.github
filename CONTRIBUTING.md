# Contributing to NumFast

Thanks for your interest! We welcome contributions of all kinds.

## How to contribute

1. **Fork** the relevant repository (NoFast, Builder, etc.)
2. **Create a branch** — `git checkout -b feature/your-feature`
3. **Write code** following the project conventions:
   - GPU-first: all numerical operations run on GPU by default
   - No CPU transfers in public API (no `.get()`, `.tolist()`, `.item()`)
   - Minimize abstractions — flat is better than nested
4. **Add tests** — test coverage is required for new features
5. **Run tests** — `python -m pytest tests/`
6. **Submit a pull request**

## Code of conduct

Be respectful, constructive, and welcoming. We're all here to learn and build great software together.

## Questions?

Open an issue or start a discussion — we're happy to help.
