# douman-ci

My scripts for CI

## Rust

- [General Rust check](.github/workflows/rust.yml) - General purpose workflow to perform checks for Rust projects
- [WASM check](.github/workflows/wasm-rust.yml) - Specialized workflow to run checks under WASM environment
- [Cross compilation check](.github/workflows/cross-rust.yml) - Specialized workflow to run checks under [cross](https://github.com/cross-rs/cross). Refer to cross's README for list of supported targets
