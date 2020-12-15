# memmap2
![Build Status](https://github.com/RazrFalcon/memmap2-rs/workflows/Rust/badge.svg)
[![Crates.io](https://img.shields.io/crates/v/memmap2-rs.svg)](https://crates.io/crates/memmap2-rs)
[![Documentation](https://docs.rs/memmap2-rs/badge.svg)](https://docs.rs/memmap2-rs)
[![Rust 1.31+](https://img.shields.io/badge/rust-1.31+-orange.svg)](https://www.rust-lang.org)

A Rust library for cross-platform memory mapped IO.

This is a **fork** of the [memmap-rs](https://github.com/danburkert/memmap-rs) crate.

## Changes

- Remove `winapi` dependency. [memmap-rs/pull/89](https://github.com/danburkert/memmap-rs/pull/89)
- Use `LICENSE-APACHE` instead of `README.md` for some tests since it's immutable.
- CI moved to GitHub Actions.
- MSRV is 1.31 now (edition 2018).

## Features

- [x] file-backed memory maps
- [x] anonymous memory maps
- [x] synchronous and asynchronous flushing
- [x] copy-on-write memory maps
- [x] read-only memory maps
- [x] stack support (`MAP_STACK` on unix)
- [x] executable memory maps
- [ ] huge page support

A list of supported/tested targets can be found in [Actions](https://github.com/RazrFalcon/memmap2-rs/actions).

## License

`memmap2` is primarily distributed under the terms of both the MIT license and the
Apache License (Version 2.0).

See [LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT) for details.

Copyright (c) 2015 Dan Burkert.
