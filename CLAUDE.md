# Claude Code Notes

@AGENTS.md

---

## Claude-specific notes

- **Default to direct tool use.** Read, Edit, Write, and Bash cover most vault work. Only reach for specialized skills if the operator asks.
- **Obsidian wikilinks** (`[[Filename]]` and `[[Filename#Heading|Display Text]]`) are preferred for in-vault references. Markdown links are fine for cross-folder readability.
- **Filenames are ASCII-only and may contain spaces.** Always quote paths in Bash. Prefer the file-editing tools over shell when possible.
- **Triage docs archive to `999-ARCHIVE/`** after execution. Don't leave them in the inbox.
