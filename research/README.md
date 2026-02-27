# Research Folder

Project: `clawdbot`

Purpose:
- Keep research outputs in one predictable place per project.
- Enable local-first lookup before web research.

Minimum standard:
1. Exactly one topic per file (no multi-topic bundles).
2. Use YAML frontmatter (start from `_template.md`).
3. Progressive disclosure sections are mandatory:
   - TL;DR
   - Key Facts
   - Recommendation
   - Deep Evidence
   - Appendix (optional)
4. File naming for agent outputs: `<topic>_[CODEX|KIMI]_YYYY-MM-DD.md`.
5. Store supporting machine-readable data as sidecars when useful (`.json`).

Suggested flow:
1. Check local memory first:
   - Claude Code: `bash /home/alex/.claude/scripts/research-memory.sh find "<query>"`
   - Codex: `bash /home/alex/.codex/scripts/research-memory.sh find "<query>"`
2. If missing/stale, do web research.
3. Save synthesized output back in this folder with metadata.
