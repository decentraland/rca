# RCA repository

Markdown only — no build, test, lint or format tooling. `/ship-it` skips Step 4a–4d here by design.

## Writing an RCA

- One file per incident: `vulnerabilities/YYYY-MM-DD.md`, suffixed `-2`, `-3` when a
  date carries more than one report. Start from `vulnerabilities/template.md`.
- Spell the month out in full, in both the `# ` heading and the metadata table:
  `August-06-2026`, not `Aug-06-2026`. The template's `Month-DD-YYYY` placeholder
  reads as an abbreviation and has produced that drift before.
- Link related incidents by relative path, e.g. `[2026-07-23](2026-07-23-2.md)`.
- The matching `template.md` (`vulnerabilities/` or `incidents/`) is the authority
  on structure: use exactly its sections and add none of your own — no
  `Verification` section, for instance; the fix's testing belongs in its PR/commits.
