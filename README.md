# rust-arduino

the purpose of this repo is to be a consortium of snippets running rust on a arduino mega board.

# initial setup

## install dep for debian

```
sudo apt install avr-libc gcc-avr pkg-config avrdude libudev-dev build-essential
```

## set toolchain

rust-toolchain.toml
```
[toolchain]
channel = "nightly-2023-08-08"
components = ["rust-src"]
profile = "minimal"
```

## install cargo tools

```
cargo install ravedude
cargo install cargo-generate
```

## apply avr-hal-template

```
cargo generate --git https://github.com/Rahix/avr-hal-template.git
```

## License
Licensed under either of

 - Apache License, Version 2.0
   ([LICENSE-APACHE](LICENSE-APACHE) or <http://www.apache.org/licenses/LICENSE-2.0>)
 - MIT license
   ([LICENSE-MIT](LICENSE-MIT) or <http://opensource.org/licenses/MIT>)

at your option.

## Contribution
Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.
