---
description: Look up a symbol in the codebase glossary — pass symbol name as argument
---

Look up a symbol in the codebase glossary.

Symbol to find: $ARGUMENTS

Steps:
1. If GLOSSARY.md doesn't exist, run: `tokalator-generate "$PWD"`
2. Search GLOSSARY.md for the symbol name (case-insensitive partial match)
3. Report: file path, line number, type, and info for each match
4. If no matches found, suggest similar names using grep
