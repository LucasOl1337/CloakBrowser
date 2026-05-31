# Changelog

## [2026-05-31] — Batch Safe Sync (Multi-Agent Reconciliation)

**Project:** CloakBrowser  
**Context:** Global 2026-05-31 batch across 12 active projects (CloakBrowser, nexarq, AutoWebGame, cortex-pessoal, LojaSync, OmniVoiceDash, PromptDE, TerminalDE, The-Last-Arrow, VideoGen, Yume, MoneyPrinterTurbo). 18 projects total showed 24h activity.

### Summary
- 5 uncommitted files focused on stealth configuration parity (Python + JS) and test coverage for timezone/locale/fingerprint injection + sandbox policy.
- Aligned with upstream v0.3.30 (Chromium 146) features: humanize, geoip, persistent contexts, 58 C++ patches.
- Local vs origin/main: 0 ahead / 0 behind on committed history; 5 dirty files (configs + tests).
- Added comprehensive 2026-05-31 patchnotes.md + this changelog entry documenting the delta + full multi-agent reconciliation.

### Added
- Expanded test matrix for new stealth flags (`--fingerprint-timezone`, `--fingerprint-locale`, timezone_id alias, override dedup).
- Detailed docstrings and policy logic in config layers.

### Changed
- cloakbrowser/config.py — version maps, get_default_stealth_args, sandbox heuristics (full parity with JS).
- js/src/config.ts — mirrored platform detection, binary paths, WRAPPER_VERSION extraction.
- tests/test_build_args.py + js/tests/config.test.ts — new coverage for launch arg injection and human-like behavior guarantees.
- patchnotes.md — full 2026-05-31 augmentation (tables, per-file analysis, agent recon section).
- changelog.md — this new top entry.

### Removed
- None.

### Local commits not on compared GitHub ref
(none — clean on committed history)

### File-level PC x GitHub delta (working tree)
M	cloakbrowser/config.py
M	js/src/config.ts
M	js/tests/config.test.ts (and related)
M	tests/test_build_args.py
M	patchnotes.md
M	changelog.md

### GitHub Comparison
- origin/main (LucasOl1337 fork): matches baseline + latest published features.
- upstream (CloakHQ/CloakBrowser): active public development; local wrapper changes are additive and compatible.
- Remotes confirmed in .git/config.

### Multi-Agent Parallel Work Notes
Multiple agents (Grok 4.3, Claude instances with .claude/.codegraph in sibling projects, prior loop/manual) worked in parallel. Common artifacts: grokassets/ rollout (per root GROKASSETS-PLAN.md 2026-05-31) for shared visual/agent tooling across most projects (CloakBrowser focused on functional config instead). Overlaps reconciled via uniform documentation + staging for central safe commit. No conflicts. Prior 2026-05-26 SP safe commit (docs-only) was the immediate baseline.

### Activity Window (last 24h)
- Stealth config + test refinements (primary)
- Docs / patchnotes / changelog augmentation (this batch)

### Notes
- Ready for clean 2026-05-31 safe commit.
- Fork relationship healthy (origin + upstream tracking preserved).
- See patchnotes.md for full executive + per-file detail + reconciliation narrative.

---

## 2026-05-26 SP safe commit
Projeto: CloakBrowser
Caminho: C:\Users\user\Desktop\CloakBrowser
Branch: main
Local HEAD antes do commit: 941f1af
Base GitHub comparada: origin/main em 941f1af (0 ahead / 0 behind).

### Added
- Nenhum item encontrado.

### Changed
-  M changelog.md
-  M patchnotes.md

### Removed
- Nenhum item encontrado.

### Local commits not on compared GitHub ref
(nenhum)

### File-level PC x GitHub delta
M	changelog.md
M	patchnotes.md

### Activity window: last 24h
- changelog.md
- patchnotes.md

### Notes
- Entrada gerada automaticamente antes do safe commit solicitado.
- O objetivo e deixar auditavel o estado local atual em comparacao com GitHub.

(End of 2026-05-31 entry. All prior history preserved above.)
