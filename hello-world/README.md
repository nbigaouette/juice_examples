# Exploration of Juice

[![Build Status](https://travis-ci.org/nbigaouette/juice_examples.svg?branch=master)](https://travis-ci.org/nbigaouette/juice_examples)

This repo contains exploration code of [Juice](https://github.com/spearow/juice),
_The Hacker's Machine Learning Engine_ (formerly known as leaf).

## macOS

On macOS, both `openblas` and `capnp` are required, through homebrew:

```sh
brew install openblas capnp
export PKG_CONFIG_PATH=/usr/local/opt/openblas/lib/pkgconfig
```

## Native

```sh
cargo run --no-default-features --features "native"
```

or simply:

```sh
cargo run
```

since `native` is the default in the `Cargo.toml` file.

## OpenCL

Note that `native` is still required:

```sh
cargo run --no-default-features --features "opencl,native"
```

## Cuda

TODO

## License

Licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.
