# Lugaru – Modernization Fork

A personal fork of the open source game [Lugaru](https://github.com/osslugaru/lugaru),
used to learn modern C++ by refactoring a real-world codebase step by step.

## About this fork

This repository is a fork of the open source game Lugaru, developed by Wolfire Games in 2005. I mainly forked it to dive deeper into C++ and practice my refactoring skills.

## Goals

As it is mainly a practice project, I do not have a clear vision or deadline. I will certainly upgrade to C++20 (to explore its new features), implement tests and CI, and a modern OpenGL renderer. After that, I will focus on skills relevant to my own profession (software development in the geosciences), such as processing digital elevation models and large rasters, and making C++ tools usable from Python.

## Status

Early stage: builds and runs like upstream; tooling is being set up.

## Building

Dependencies are listed in [COMPILING.md](COMPILING.md). On Linux:

```bash
cmake -B build -G Ninja -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_EXPORT_COMPILE_COMMANDS=ON
cmake --build build
./build/lugaru
```

## Contributing

Right now, I welcome helpful contributions and discussions. Please open an issue before opening a pull request, and keep in mind that this fork mainly exists to practice refactoring and explore modern C++.

## License and credits

Code: GPL-2.0-or-later ([COPYING.txt](COPYING.txt)) · Assets: CC-BY-SA ([CONTENT-LICENSE.txt](CONTENT-LICENSE.txt)) · Original: Wolfire Games / [osslugaru](https://github.com/osslugaru/lugaru) · Original README: [Docs/README-upstream.md](Docs/README-upstream.md)
