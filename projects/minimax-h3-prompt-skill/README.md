# MiniMax H3 Prompt Compiler Skill

This directory is reserved for public-safe project handovers, decisions, audit reports, regression evidence, and release records for the MiniMax H3 Prompt Compiler Skill.

## Archive policy
- Treat the user's designated source ZIP as authoritative when explicitly identified.
- Keep source packages, runtime packages, reports, and test evidence distinct.
- Record exact package versions and SHA-256 values from verified artifacts only.
- Distinguish static checks, host/skill-loading checks, and actual H3 generation tests.
- Do not label a candidate as stable unless the recorded release criteria support it.
- Keep user-confirmed requirements separate from assistant recommendations.
- Do not commit private conversation transcripts or secrets to this public repository.

## Suggested directory layout

```text
minimax-h3-prompt-skill/
├── README.md
├── handover.md
├── decisions/
├── conversations/
├── audits/
├── tests/
└── releases/
```

## Current state

This is an archive index only. No skill ZIP, private conversation transcript, audit report, or release artifact has been copied into this directory yet. Add materials only after verifying the source and confirming they are safe for this public repository.

## Required evidence labels

- **Verified:** directly checked against the artifact or test output.
- **Partially verified:** some checks passed, with explicit limits.
- **Reported, not independently verified:** a person or prior AI stated it, but the underlying evidence has not been checked.
- **Inferred:** a reasoned conclusion, not a direct source fact.
