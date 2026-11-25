# STM32F3DISCOVERY

Minimal bare-metal Rust firmware for the STM32F3 Discovery board (`STM32F303VCTx`). 

## Build

With Rust and Cargo installed via rustup, add the target and build from the repository root. Cargo selects the target automatically.

```sh
rustup target add thumbv7em-none-eabihf
cargo build
```

## Flash and run

Install the `probe-rs` CLI and connect the board to your computer through its onboard ST-LINK USB port. Then run:

```sh
cargo run
```

The runner in `.cargo/config.toml` uses `probe-rs` to flash and start the firmware.
