
-# this is just for the meme, i didn't even test it but i mean it maybe works
# I use Windows btw

> "I use Windows btw" but it's a Turing-complete programming language.

## Introduction

I use Windows btw is an esoteric programming language based on [Brainfuck](
https://en.wikipedia.org/wiki/Brainfuck) in which the commands are the following
keywords:

`i`, `use`, `windows`, `10`, `btw`, `by`, `the`, `way`, `windowsME`.

See the [language specification](./docs/language_specification.md) for more
information.

This repository contains a [C/C++ library implementing I use Arch btw](./lib)
and a dependent [command-line interpreter](./cmd).

## Getting Started

### Prerequisites

- [CMake](https://cmake.org/) >= 3.23
- a C99 and C++17 compiler toolchain supported by CMake and providing POSIX
  [`unistd.h`](https://en.wikipedia.org/wiki/Unistd.h), `mmap()`, `MAP_ANON`,
  and defining `__x86_64__` when targeting x86-64

### Building

    $ mkdir build
    $ cd build
    $ cmake -DCMAKE_BUILD_TYPE=Release -DBUILD_SHARED_LIBS=ON ..
    $ cmake --build .

### Installation

    # cmake --install .

### Usage

#### Command-line interpreter

    $ i-use-windows-btw <source file>

Try some of the [example I use Windows btw programs](./examples) as source files.

For details:

    $ i-use-windows-btw -h

#### C/C++ library

For documentation of the public API, see the [public headers](
./lib/include/iuab).

For example usage, see the [command-line interpreter](./cmd) and [example
libiuab programs](./examples/libiuab).

## License

This software is licensed under the [GNU General Public License, version 3](
./LICENSE.md).
