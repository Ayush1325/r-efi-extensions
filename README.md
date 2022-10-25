r-efi-extensions
=====

Rust specific extensions for [r-efi](https://github.com/r-efi/r-efi) crate

This crate defines Rust specific extensions for r-efi crate. This does not aim to be a user-friendly wrapper around r-efi but rather provide some functionality which
1. Can simply not be represented in the C way (Variable argument functions: see [r-efi/issues/12](https://github.com/r-efi/r-efi/issues/12))
2. Provide quality of life improvements for Rust.

### Requirements

The requirements for this project are:

 * `rustc >= 1.51.0`

### Build

To build this project, run:

```sh
cargo build
```

No special requirements exist to compile for UEFI targets. Native compilations
work out of the box without any adjustments. For cross-compilations, you have
to use either `cargo-xbuild` or the nightly versions of `cargo` and `rustc`. In
both cases, you need a nightly toolchain and the compiler sources:

```sh
rustup toolchain install nightly
# OR
rustup update

rustup component add --toolchain nightly rust-src
```

Be sure to update all components to the most recent version.

### License:

 - **MIT** OR **Apache-2.0** OR **LGPL-2.1-or-later**
 - See AUTHORS file for details.
