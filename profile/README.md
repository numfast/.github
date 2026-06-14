# NumFast

**GPU-accelerated numerical computing, from Python to browser.**

NumFast is a family of open-source libraries for high-performance numerical computing:

- **[NoFast](https://github.com/numfast/numfast)** — Python framework for GPU numerical computing on CuPy. Same code runs on CPU (NumPy) when CUDA is unavailable.
- **[Builder](https://github.com/numfast/framework-builder)** — Lightweight meta-framework for assembling NumFast applications from manifests and extensions.
- **[NoFast.js](https://github.com/numfast/numfast-js)** (coming soon) — Browser-based GPU computing via WebGPU with transparent CPU fallback.

## Why NumFast?

- **GPU-native design** — not an afterthought. Every operation runs on GPU by default.
- **Write once, run anywhere** — single codebase for CUDA (Python), CPU (NumPy), and WebGPU (browser).
- **Minimal dependencies** — NoFast depends only on CuPy; Builder has zero runtime dependencies.
- **Simple architecture** — Understandable in 2 minutes. No deep abstraction chains.

## License

All NumFast projects are open-source under the [MIT License](LICENSE).
