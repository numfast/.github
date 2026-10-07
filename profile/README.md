# NumFast

**Columnar compute for Python and JavaScript — native CPU and GPU, WebAssembly
kernels, and browser execution.**

NumFast is a small family of open-source libraries:

- **[NumFast](https://github.com/numfast/numfast)** — the columnar compute engine.
  Python and JavaScript, with native CPU and GPU kernels, a WebAssembly kernel
  library, and browser execution.
  · [PyPI](https://pypi.org/project/numfast/) ·
  [npm](https://www.npmjs.com/package/@numfast/kernels) ·
  [install guide](https://github.com/numfast/numfast/blob/main/docs/INSTALL.md)
- **[App Builder](https://github.com/numfast/app-builder)** — the extension
  framework NumFast is itself built from: manifest-driven modules assembled at
  load time, in Python and in TypeScript.

## What NumFast actually does today

- **Columnar engine** — a `Table` of columns with an explicit NULL, integer
  arithmetic exact in `int32`, and a lazy query chain the planner turns into one
  execution graph.
- **Native CPU** — Rust kernels loaded through `ctypes`, shipped as a Windows
  wheel and a `manylinux_2_28_x86_64` wheel. No Rust toolchain is needed to
  install it.
- **GPU** — 15 of 33 operations run on the GPU through WebGPU. The recorded
  measurements are **slower than the CPU path at the sizes measured**; no speedup
  is claimed, and there is no GPU-resident table.
- **WebAssembly and browser** — the kernels compile to an 86-function module
  with one memory and no imports. It runs in Node and in the browser. It is a
  **kernel library, not a compute engine**: there is no WASM executor.
- **Honest performance** — where NumFast loses, it says so. High-cardinality
  grouping is several times behind DuckDB.

## Licence

NumFast and App Builder are **AGPL-3.0-only**. The `.github` templates in this
repository (issue and pull-request templates, `CONTRIBUTING.md`) are MIT.
See [LICENSING.md](LICENSING.md).
