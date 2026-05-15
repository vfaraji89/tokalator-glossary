# tokalator-glossary

A Claude Code plugin that auto-generates a codebase glossary (symbol index) after `/init` or on demand. Saves tokens by giving Claude a compressed map of your entire codebase.

## Install

**Local testing:**
```bash
claude --plugin-dir ./tokalator-glossary
```

**From GitHub marketplace:**
```
/plugin marketplace add vfaraji89/tokalator-glossary
/plugin install tokalator-glossary
```

**CLI install:**
```bash
claude plugin install tokalator-glossary@vfaraji89
```

## Commands

| Command | Description |
|---------|-------------|
| `/tokalator-glossary:glossary` | Generate full glossary |
| `/tokalator-glossary:glossary-lookup <name>` | Find a symbol |
| `/tokalator-glossary:glossary-stats` | Codebase statistics |
| `/tokalator-glossary:glossary-refresh` | Regenerate after changes |

## Auto-trigger

The plugin hooks into `PostToolUse` — when `/init` writes `CLAUDE.md`, the glossary generates automatically in the background.

## Output

Generates `GLOSSARY.md` at the project root with:
- Symbol count and file count summary
- Per-file table of classes, functions, constants
- File path, line number, and signature for each symbol

## Supported Languages

| Language | Extensions |
|----------|-----------|
| Python | `.py` |
| JavaScript | `.js`, `.jsx` |
| TypeScript | `.ts`, `.tsx` |

## License

MIT
