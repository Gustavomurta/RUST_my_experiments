
### A Rust Embedded-HAL implementation for the rp2040 microcontroller:

https://crates.io/crates/rp2040-hal



### Getting Started:

`rustup self update`

`rustup update stable`

`rustup target add thumbv6m-none-eabi`

Useful to creating UF2 images for the RP2040 USB Bootloader:

`cargo install elf2uf2-rs --locked`

https://github.com/rp-rs/rp-hal/tree/main



### RP2040 hal examples: 

https://github.com/rp-rs/rp-hal/tree/main/rp2040-hal-examples

### Getting Started
To build all the examples, first grab a copy of the source code:

`git clone https://github.com/rp-rs/rp-hal.git`

Then use rustup to grab the Rust Standard Library for the appropriate target and our preferred flashing tool:

`rustup target add thumbv6m-none-eabi`

Then you can build the examples:

`cd rp2040-hal-examples`

`cargo build`

`cargo build --bin pio-blink`   (Compile pio-blink.rs example) 

`cargo install elf2uf2-rs --locked` (Install flash tool) 

`Boot your RP2040 into "USB Bootloader mode", typically by rebooting whilst holding "Boot Select" button`

`cargo run --bin pio-blink`     (Compile and flash pio-blink.rs example)







