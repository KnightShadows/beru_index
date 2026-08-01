# Beru Global Registry Index

This repository acts as the central registry for the **Beru** package manager. It contains `recipe.toml` files that instruct the Beru build engine how to fetch, compile, and link third-party C++ dependencies.

## Structure

Packages in this index follow a strict directory structure:
`<package_name>/<version>/recipe.toml`

Example:
```
fmt/
└── 11.0.2/
    └── recipe.toml
```

## Contributing a Package

To add a new library or version to the global index:

1. Fork this repository.
2. Create the appropriate `<package_name>/<version>` directory.
3. Add a valid `recipe.toml` file containing `[package]`, `[source]`, `[build]`, and `[export]` blocks.
4. Submit a Pull Request!

### Example `recipe.toml`

```toml
[package]
name = "fmt"
version = "11.0.2"

[source]
git = "https://github.com/fmtlib/fmt.git"
tag = "11.0.2"

[build]
system = "cmake"
args = ["-DFMT_TEST=OFF", "-DFMT_DOC=OFF"]

[export]
include_dirs = ["include"]
libs = ["fmt"]
```

## Usage

When you list a dependency in your local `Beru.toml`, the `beru` CLI automatically downloads a shallow clone of this index to `~/.beru/index`, searches for the highest compatible version, and parses the recipe to build your dependency.
