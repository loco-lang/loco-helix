[![CI](https://github.com/loco-lang/loco-helix/actions/workflows/ci.yml/badge.svg)](https://github.com/loco-lang/loco-helix/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

# loco-helix

Helix editor configuration for the [Loco](https://github.com/loco-lang/loco) programming language.

**This is a mirror repo.** The canonical source is maintained in
[tree-sitter-loco/editors/helix](https://github.com/loco-lang/tree-sitter-loco/tree/main/editors/helix).

To update: submit changes to `tree-sitter-loco/editors/helix/`, and they will be synced here.

## Installation

Add to `~/.config/helix/languages.toml`:

```toml
[[language]]
name = "loco"
scope = "source.loco"
file-types = ["loco"]
comment-token = "//"
indent = { tab-width = 4, unit = "\t" }

[[grammar]]
name = "loco"
source = { git = "https://github.com/loco-lang/tree-sitter-loco", rev = "main" }
```

Copy query files to `~/.config/helix/runtime/queries/loco/`.

## Related

- [Tree-sitter grammar](https://github.com/loco-lang/tree-sitter-loco)
- [All editor extensions](https://github.com/loco-lang/tree-sitter-loco#editor-support)

## License

MIT
