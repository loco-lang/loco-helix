[![CI](https://github.com/loco-lang/loco-helix/actions/workflows/ci.yml/badge.svg)](https://github.com/loco-lang/loco-helix/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

# Loco for Helix

Loco language support for the [Helix editor](https://helix-editor.com).

## Features

- Syntax highlighting
- Code folding
- Symbol outline / navigation
- Text object selections
- Scope-aware highlighting

## Installation

### With the tree-sitter grammar auto-download

Add this to your `~/.config/helix/languages.toml`:

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

### Manual query files

If you prefer to use the query files directly:

```bash
cp -r runtime/* ~/.config/helix/runtime/
```

## Updating queries

The `.scm` query files here are sourced from [tree-sitter-loco](https://github.com/loco-lang/tree-sitter-loco/queries/).
To update, copy the latest from that repo.

## License

MIT
