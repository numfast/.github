# NumFast

**GPU-accelerated numerical computing, from Python to browser.**

NumFast is a family of open-source libraries for high-performance numerical computing:

- **[NumFast](https://github.com/numfast/numfast)** — GPU-first numerical framework for Python. WebGPU backend for browsers via `@numfast/numfast` on npm.
- **[Builder](https://github.com/numfast/framework-builder)** — Lightweight meta-framework for assembling NumFast applications from manifests and extensions.

## Why NumFast?

- **GPU-native design** — not an afterthought. Every operation runs on GPU by default.
- **Python + JavaScript parity** — same API, same deterministic random (PCG-u32), bit-exact results.
- **Minimal dependencies** — NumFast depends only on numpy + wgpu; Builder has zero runtime dependencies.
- **Honest performance** — measured numbers only, published in [docs/PERFORMANCE.md](https://github.com/numfast/numfast/blob/main/docs/PERFORMANCE.md).

## License

All NumFast projects are open-source under the [MIT License](LICENSE).
