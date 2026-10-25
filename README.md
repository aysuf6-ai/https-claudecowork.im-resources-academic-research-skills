# Academic Research Skills (selected copy)

This repository holds a selected copy of five Claude skills from
[Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)
by Cheng-I Wu, taken at upstream commit `77e77e8` (2026-10-25).

## Attribution and license

All skill content is © 2026 Cheng-I Wu and is used under the
[Creative Commons Attribution-NonCommercial 4.0 International License](LICENSE).
It is copied without changes. Non-commercial use only. See [NOTICE.md](NOTICE.md)
for the author's statement.

## What is included

| Folder | Purpose |
|---|---|
| `deep-research/` | Literature reviews, systematic reviews, fact-checking, Socratic research-question dialogue |
| `academic-paper/` | Paper drafting, outlining, revision, citation checks, AI-use disclosure, rebuttal audit |
| `academic-paper-reviewer/` | Simulated multi-reviewer peer review panel |
| `academic-pipeline/` | Orchestrates research, writing, review and revision end to end |
| `sr-screener/` | Protocol-driven PRISMA screening for systematic reviews |
| `shared/` | Shared references used by the skills above (linked as `../shared/`) |
| `MODE_REGISTRY.md` | Index of every skill mode |

The upstream `docs/`, `scripts/`, `agents/`, `commands/`, `examples/`, `tests/` and
`.github/` folders were left out on purpose, so a few cross-links inside the skills
point to files that are not in this copy. Those files can be read in the upstream
repository.

## Installing

Each skill must sit at `.claude/skills/<skill-name>/SKILL.md` for Claude Code to find
it. From a project folder:

```bash
git clone https://github.com/aysuf6-ai/https-claudecowork.im-resources-academic-research-skills.git ~/ars
mkdir -p .claude/skills
for s in deep-research academic-paper academic-paper-reviewer academic-pipeline sr-screener; do
  ln -s ~/ars/$s .claude/skills/$s
done
```

Keep the clone intact so the `../shared/` links resolve. For claude.ai or Cowork,
zip each skill folder and upload it through the skills settings.
