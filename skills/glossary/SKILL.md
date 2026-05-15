---
description: Generate a full codebase glossary (symbol index) for the current project
---

Generate a codebase glossary using the tokalator engine.

Steps:
1. Run: `tokalator-generate "$PWD"`
2. Read the generated GLOSSARY.md
3. Give a brief summary: total symbols, files scanned, top-level structure
4. If GLOSSARY.md already exists, ask whether to regenerate or show the existing one
5. Add to CLAUDE.md if not already present:
   ```
   ## Tokalator Glossary
   See GLOSSARY.md for auto-generated symbol index. Consult before exploring files.
   ```
