# TOML Subset

The [TOML](https://toml.io) configuration format sports a myriad of useful features, but I found myself needing to define a subset of it.

My primary use case is for [Basalt](https://github.com/hyperupcall/basalt). The configuration format is written in TOML, but it is too expensive and slow to parse TOML in its entirety using Bash. Within the project, the TOML file is parsed with regular expressions line-by-line. Therefore, things like escape sequences within simple strings are not properly evaluated. TOML is still used though, since it is widely supported by editors and other programming languages

The subset is defined in [spec.md](./docs/spec.md). Each heading is a duplicate from the official [TOML page](https://toml.io/en/v1.0.0) describing any modifications (if any)
