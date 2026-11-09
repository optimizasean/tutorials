# tutorials

Tutorials, learning, training, and exercises, organized alphabetically by language,
then by provider or tutorial repository. Each tutorial is a Git submodule.

## Directory structure

```text
.
├── ruby/
│   └── Depot/
├── rust/
│   └── rustlings/
├── typescript/
│   └── total-typescript/
│       ├── pro-essentials-workshop/
│       └── type-transformations-workshop/
├── wasm/
│   └── watlings/
└── zig/
    └── ziglings/
```

Repository folder names are retained so they are easy to match to their sources.

## Tutorials and sources

The **source** links point to the original tutorials or upstream projects. The
**checkout repository** links show where the submodules are cloned from, including
personal forks used to track progress.

| Local path | Tutorial / original source | Checkout repository |
| --- | --- | --- |
| [`ruby/Depot`](ruby/Depot) | The Depot Application, Chapter 5 of [Agile Web Development with Rails](https://www.oreilly.com/library/view/agile-web-development/9780976694007/) | [optimizasean/Depot](https://github.com/optimizasean/Depot) |
| [`rust/rustlings`](rust/rustlings) | [Rustlings](https://github.com/rust-lang/rustlings) — small Rust exercises | [optimizasean/rustlings](https://github.com/optimizasean/rustlings) |
| [`typescript/total-typescript/pro-essentials-workshop`](typescript/total-typescript/pro-essentials-workshop) | [TypeScript Pro Essentials](https://github.com/total-typescript/pro-essentials-workshop) | [optimizasean/pro-essentials-workshop](https://github.com/optimizasean/pro-essentials-workshop) |
| [`typescript/total-typescript/type-transformations-workshop`](typescript/total-typescript/type-transformations-workshop) | [Type Transformations](https://github.com/total-typescript/type-transformations-workshop) | [optimizasean/type-transformations-workshop](https://github.com/optimizasean/type-transformations-workshop) |
| [`wasm/watlings`](wasm/watlings) | [Watlings](https://github.com/EmNudge/watlings) — WebAssembly Text Format exercises | [optimizasean/watlings](https://github.com/optimizasean/watlings) |
| [`zig/ziglings`](zig/ziglings) | [Ziglings](https://codeberg.org/ziglings/exercises) — small Zig exercises | [optimizasean/ziglings](https://github.com/optimizasean/ziglings) |

## Getting started

Clone this repository with its tutorials:

```sh
git clone --recurse-submodules git@github.com:optimizasean/tutorials.git
```

For an existing clone, initialize the tutorials at the recorded commits:

```sh
git submodule update --init --recursive
```

See each tutorial's README for its dependencies and exercise commands.
[`.gitmodules`](.gitmodules) lists the checkout URLs, directory paths, and branch
settings in the same order as the tree above. Git uses each submodule's `path`
setting for its location; its section name is a stable identifier and may retain
an older path after a move.
