# AI- — AI Conversation & Project Archive

This repository is a structured archive for AI-assisted projects, important user conversations, project decisions, handovers, research, and verification records.

## Repository structure

```text
AI-/
├── README.md
├── .gitignore
├── templates/
│   ├── CONVERSATION-ARCHIVE-TEMPLATE.md
│   └── PROJECT-HANDOVER-TEMPLATE.md
└── projects/
    ├── README.md
    └── minimax-h3-prompt-skill/
        └── README.md
```

## How to use it

1. Create a separate directory under `projects/` for each substantial project.
2. Use the conversation archive template for important conversation records.
3. Use the project handover template to preserve current state and continue work across new AI chats.
4. Keep source transcripts, summaries, decisions, reports, and release artifacts distinguishable.
5. Record exact paths, versions, commit IDs, hashes, and test evidence when they matter.
6. Mark claims as **verified**, **reported but unverified**, or **inferred**. Never present an untested claim as a completed test.
7. Update the project handover after major decisions or releases.

## Privacy and security

**This repository is public.** Only commit material that is safe for anyone to read.

- Do not upload passwords, API keys, access tokens, recovery codes, private URLs, or credentials.
- Do not publish private raw conversation transcripts, personal information, confidential business material, or other sensitive content.
- Redact or summarize private conversations before archiving them here.
- The `.gitignore` file is only a safeguard; it does not guarantee that sensitive files will be excluded.
- If private conversation storage is required, change the repository to **Private** before uploading that material.
- If a secret is accidentally committed, removing it from the latest file is not enough; revoke/rotate the secret and clean the Git history as needed.

## Archive quality rules

- Preserve the user's confirmed wording and intent where important.
- Separate confirmed decisions from suggestions and assumptions.
- Keep historical records; mark superseded material instead of silently rewriting history.
- Treat the designated source artifact as authoritative when a project explicitly establishes one.
- Keep audit evidence and generated deliverables separate.
- Avoid copying an entire chat when a concise, faithful record is sufficient and safe.

## Templates

- [Conversation Archive Template](templates/CONVERSATION-ARCHIVE-TEMPLATE.md)
- [Project Handover Template](templates/PROJECT-HANDOVER-TEMPLATE.md)

## Projects

- [Projects Archive Guide](projects/README.md)
- [MiniMax H3 Prompt Compiler Skill](projects/minimax-h3-prompt-skill/README.md)

## Maintenance

This structure is the initial baseline. Add project-specific directories only when needed, and keep the root README synchronized with major structural changes.
