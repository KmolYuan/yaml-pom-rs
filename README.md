# yaml-peg

[![dependency status](https://deps.rs/repo/github/KmolYuan/yaml-peg-rs/status.svg)](https://deps.rs/crate/yaml-peg/)

A YAML 1.2 parser using greedy parsing algorithm with PEG atoms. Support anchor visitor and no-std.

Inspired from [`yaml-rust`](https://github.com/chyh1990/yaml-rust).

This parser is not ensure about YAML spec but almost functions are well-implemented. The buffer reader has also not yet been implemented, but the chunks can be read by sub-parsers.

See the API doc for more information.

## Features

+ Support no standard library `#![no_std]`.
+ Support anchor visitor through reference counter.
+ Different data holder provides parallel visiting and less copy cost.
