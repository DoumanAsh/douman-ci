# douman-ci

My scripts for CI

## Actions

- [Trivy Vulnerability Report](.github/actions/trivy-report-vuln/action.yaml) - Composite action to check and report docker image vulnerabilities using Trivy. [Example](https://github.com/DoumanAsh/nginx-sftp/blob/c8f384ccc5502e89b3390fdbea5cf7ff5f6bf9dc/.github/workflows/docker-image.yml#L126)

## Workflows

### Rust

- [General Rust check](.github/workflows/rust.yml) - General purpose workflow to perform checks for Rust projects. [Example](https://github.com/DoumanAsh/str-buf/blob/d5a185ce83ee414a045c533980fb57adf4d5c524/.github/workflows/rust.yml#L21)
- [WASM check](.github/workflows/wasm-rust.yml) - Specialized workflow to run checks under WASM environment. [Example](https://github.com/DoumanAsh/xxhash-rust/blob/a8108b485f612f20d4bca7500c89f1b0be140971/.github/workflows/rust.yml#L112)
- [Cross compilation check](.github/workflows/cross-rust.yml) - Specialized workflow to run checks under [cross](https://github.com/cross-rs/cross). Refer to cross's README for list of supported targets. [Example](https://github.com/DoumanAsh/xxhash-rust/blob/a8108b485f612f20d4bca7500c89f1b0be140971/.github/workflows/rust.yml#L133)
- [Rust Release workflow](.github/workflows/release-rust.yaml) - General purpose workflow to release Rust binaries for Windows, Mac and Linux (including musl)

### Opentofu

- [General Tofu check](.github/workflows/tofu.yml) - General purpose workflow to perform checks for opentofu modules. [Example](https://github.com/DoumanAsh/aws-tf/blob/38bd3137030452c707b2f082a2a49cb616b606ed/.github/workflows/tofu.yaml#L21)
