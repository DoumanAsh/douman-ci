# douman-ci

My scripts for CI

## Actions

- [Trivy Vulnerability Report](.github/actions/trivy-report-vuln/action.yaml) - Composite action to check and report docker image vulnerabilities using Trivy. [Example](https://github.com/DoumanAsh/nginx-sftp/blob/3ed7a2e65538f010986a5048306151bfb4dfaa78/.github/workflows/docker-image.yml#L23-L70)

## Workflows

### Containers

- [Container image release](.github/workflows/release-container.yaml) - General purpose workflow to release container image onto most well known public registries. [Example](https://github.com/DoumanAsh/rust-musl/blob/3c97df0b1d5d460a1c19e2383bbf588fc3c0b2c6/.github/workflows/docker-image.yml#L30-L73)

### Rust

- [General Rust check](.github/workflows/rust.yml) - General purpose workflow to perform checks for Rust projects. [Example](https://github.com/DoumanAsh/str-buf/blob/d5a185ce83ee414a045c533980fb57adf4d5c524/.github/workflows/rust.yml#L21)
- [WASM check](.github/workflows/wasm-rust.yml) - Specialized workflow to run checks under WASM environment. [Example](https://github.com/DoumanAsh/xxhash-rust/blob/a8108b485f612f20d4bca7500c89f1b0be140971/.github/workflows/rust.yml#L112)
- [Cross compilation check](.github/workflows/cross-rust.yml) - Specialized workflow to run checks under [cross](https://github.com/cross-rs/cross). Refer to cross's README for list of supported targets. [Example](https://github.com/DoumanAsh/xxhash-rust/blob/a8108b485f612f20d4bca7500c89f1b0be140971/.github/workflows/rust.yml#L133)
- [Rust Release binaries](.github/workflows/release-rust.yaml) - General purpose workflow to release Rust binaries for Windows, Mac and Linux (including musl). [Example](https://github.com/DoumanAsh/conn-test/blob/9ce3309d1099c6a60dd7199e597ed26bdf40b62d/.github/workflows/release.yml#L19-L29)

### Opentofu

- [General Tofu check](.github/workflows/tofu.yml) - General purpose workflow to perform checks for opentofu modules. [Example](https://github.com/DoumanAsh/aws-tf/blob/38bd3137030452c707b2f082a2a49cb616b606ed/.github/workflows/tofu.yaml#L21)
