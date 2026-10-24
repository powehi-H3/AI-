# Archive Metadata Standard

This document defines a small, human-readable metadata standard for conversation and project records. It is a convention, not an automated validator.

## Required fields

| Field | Meaning | Example |
|---|---|---|
| archive_id | Stable unique ID; lowercase kebab-case | 2026-10-24-h3-version-audit |
| record_type | conversation / handover / decision / audit / research / release | handover |
| created | Record creation date, ISO 8601 | 2026-10-24 |
| project | Stable project slug | minimax-h3-prompt-skill |
| source | Source platform, file path, URL, or commit | GitHub URL |
| sensitivity | public-safe / redacted / private | redacted |
| verification | verified / partially-verified / unverified / inferred | partially-verified |

## Recommended fields

- `title`: short human-readable title
- `updated`: date of last material update
- `related_records`: IDs of connected records
- `related_artifacts`: paths, URLs, version IDs, and hashes
- `supersedes`: ID of a record this replaces
- `tags`: concise topic labels

## Example front matter

```yaml
---
archive_id: 2026-10-24-example
record_type: conversation
created: 2026-10-24
project: example-project
source: "source conversation URL or export path"
sensitivity: redacted
verification: partially-verified
tags:
  - handover
  - decision
---
```

## Rules

1. Use dates in `YYYY-MM-DD` format.
2. Do not use a filename as proof that the underlying content was verified.
3. Keep the source and verification status visible.
4. Never mark assistant-generated interpretations as user-confirmed unless the conversation supports that.
5. Do not commit private records to a public repository.
6. Avoid storing credentials, access tokens, passwords, recovery codes, or unnecessary personal information.
7. If a record changes materially, update its `updated` field and note the change history.
8. Hashes must be calculated from the actual artifact bytes; never estimate or copy a hash from an unrelated version.
