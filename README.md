# Freshdesk app with Rust WASM

An experimental Freshdesk app that uses [Rust to build a WebAssembly (WASM)](https://rustwasm.github.io/) component.

## Pre-requisites

1. Working knowledge of JavaScript, HTML, CSS, and Node.js.
2. Basic familiarity with Rust and WASM.
2. Basic idea on how Freshworks app development works. See [tutorials](https://developers.freshworks.com/tutorials/) for help.

## Setup

1. [Setup FDK — The Freshworks CLI](https://developers.freshdesk.com/v2/docs/quick-start/)
1. [Install the Rust toolchain](https://www.rust-lang.org/tools/install)
2. [Install wasm-pack](https://rustwasm.github.io/wasm-pack/installer/)

## Directory structure

- `app/` — The `app` directory contains frontend component of the Freshdesk app
- `rust-wasm/` - The `rust-wasm` directory contains a Rust `crate` (project) with WASM configured

## Build

### Build Rust crate

To build the Rust crate, run:

```
cd rust-wasm/
wasm-pack build
```

This will produce compiled WebAssembly files with JavaScript bindings in the `rust-wasm/pkg/` directory.