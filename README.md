```ruby
███╗   ███╗███████╗████████╗
████╗ ████║██╔════╝╚══██╔══╝
██╔████╔██║███████╗   ██║
██║╚██╔╝██║╚════██║   ██║
██║ ╚═╝ ██║███████║   ██║
╚═╝     ╚═╝╚══════╝   ╚═╝
```


## What It Does

- Strip metadata from JPEG, PNG, PDF, Word, Excel, and PowerPoint files
- Concurrent processing with ThreadPoolExecutor handles 1000+ files efficiently
- Dry-run mode previews what would be removed before making changes
- Verification reports show before/after comparison of metadata fields
- Smart format detection uses file signatures, not extensions
- Removes GPS coordinates, author info, timestamps, camera data, and software traces

## Quick Start

```bash
uv tool install metadata-scrubber
mst scrub photo.jpg
```

> [!TIP]
> This project uses [`just`](https://github.com/casey/just) as a command runner. Type `just` to see all available commands.
>
> Install: `curl -sSf https://just.systems/install.sh | bash -s -- --to ~/.local/bin`

## Commands

| Command | Description |
|---------|-------------|
| `mst read <file>` | Inspect metadata fields present in a file |
| `mst scrub <file>` | Remove all metadata from a file |
| `mst verify <file>` | Confirm metadata was successfully removed |

## Learn

This project includes step-by-step learning materials covering security theory, architecture, and implementation.

| Module | Topic |
|--------|-------|
| [00 - Overview](learn/00-OVERVIEW.md) | Prerequisites and quick start |
| [01 - Concepts](learn/01-CONCEPTS.md) | Security theory and real-world breaches |
| [02 - Architecture](learn/02-ARCHITECTURE.md) | System design and data flow |
| [03 - Implementation](learn/03-IMPLEMENTATION.md) | Code walkthrough |
| [04 - Challenges](learn/04-CHALLENGES.md) | Extension ideas and exercises |


