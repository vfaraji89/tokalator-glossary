---
description: Show codebase statistics from the glossary — files, symbols, refactor candidates
---

Show codebase statistics from the glossary.

Steps:
1. If GLOSSARY.md doesn't exist, run: `tokalator-generate "$PWD"`
2. Read GLOSSARY.md
3. Present a summary table: files by extension, symbols by type, largest files by symbol count
4. Highlight any files with 10+ symbols as candidates for refactoring
