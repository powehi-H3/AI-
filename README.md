# AI- — AI Conversation & Project Archive

This repository is a structured archive for AI-assisted projects, important user conversations, project decisions, handovers, research, and verification records.

## Repository structure

```text
AI-/
├── README.md
├── .gitignore
├── schemas/
│   └── ARCHIVE-METADATA-SCHEMA.md
├── templates/
│   ├── CONVERSATION-ARCHIVE-TEMPLATE.md
│   ├── PROJECT-HANDOVER-TEMPLATE.md
│   └── DECISION-LOG-TEMPLATE.md
└── projects/
    ├── README.md
    └── minimax-h3-prompt-skill/
        └── README.md
```

## Start here

1. For a conversation record, copy the [Conversation Archive Template](templates/CONVERSATION-ARCHIVE-TEMPLATE.md).
2. To continue a project in a new AI chat, use the [Project Handover Template](templates/PROJECT-HANDOVER-TEMPLATE.md).
3. To record a confirmed decision, use the [Decision Log Template](templates/DECISION-LOG-TEMPLATE.md).
4. Follow the [Archive Metadata Standard](schemas/ARCHIVE-METADATA-SCHEMA.md) so records can be searched and cross-linked consistently.
5. Put project records in a dedicated directory under `projects/`; see the [Projects Archive Guide](projects/README.md).

## Evidence and provenance rules

- Keep raw source records separate from summaries and conclusions.
- Distinguish user-confirmed decisions, assistant suggestions, reported claims, and inferences.
- Use explicit evidence labels: **Verified**, **Partially verified**, **Reported, not independently verified**, or **Inferred**.
- Record exact artifact versions, paths, commit IDs, and hashes only when verified against the actual source.
- Preserve historical records and mark superseded records rather than silently rewriting them.
- Do not treat an archive's filename or a prior AI's statement as proof that a test was run.

## Privacy and security

**This repository is public.** Only commit material that is safe for anyone to read.

- Do not upload passwords, API keys, access tokens, recovery codes, private URLs, or credentials.
- Do not publish private raw conversation transcripts, personal information, confidential business material, or other sensitive content.
- Redact or summarize private conversations before archiving them here.
- The `.gitignore` file is only a safeguard; it does not guarantee that sensitive files will be excluded.
- If private conversation storage is required, change the repository to **Private** before uploading that material.
- If a secret is accidentally committed, removing it from the latest file is not enough; revoke/rotate the secret and clean the Git history as needed.

## Current scope

This repository currently contains the archive framework and templates. Project-specific historical conversations, source archives, and release artifacts should be added only after their contents and public-sharing suitability are checked.

## Maintenance

After major project decisions or releases, update the project's handover and decision log. Keep this root README synchronized with changes to the archive structure.
