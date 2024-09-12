# Kartoffel

Starter pack for a 🥔 [kartoffels](https://github.com/Patryk27/kartoffels) 🥔
bot.

## Usage

Clone this repository, run `./build` (Linux / Mac) or `./build.bat` (Windows)
and then upload `./kartoffel` into [the game](https://kartoffels.pwy.io).

(if you're more into terminals, go with `ssh kartoffels.pwy.io`)

Note that this repository provides a skeleton robot meant for the in-game
tutorial - it probably won't survive long when deployed directly onto the
battlefield.

## Caveat Emptor

When implementing a kartoffel you're essentially creating a firmware, so you
don't have access to `std` - no `std::fs`, no `println!()` etc. You can
communicate through `serial_send()`, though, and you can use various fancy
structures like `Vec` through the `alloc` crate.

You're given 64 KHz CPU and 128 KiB of RAM, have fun.

## License

CC0 1.0 Universal

The person who associated a work with this deed has dedicated the work to the
public domain by waiving all of his or her rights to the work worldwide under
copyright law, including all related and neighboring rights, to the extent
allowed by law.

You can copy, modify, distribute and perform the work, even for commercial
purposes, all without asking permission.
