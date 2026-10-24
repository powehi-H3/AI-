# Projects Archive

Store each AI project in its own directory.

Suggested contents:
- `README.md`: concise project index and current status.
- `handover.md`: latest handover summary.
- `decisions/`: confirmed decisions and rationale, using the decision log template.
- `conversations/`: sanitized conversation summaries or transcripts approved for this repository.
- `audits/`: static audits and source reviews.
- `tests/`: test cases, outputs, and test reports.
- `releases/`: release notes and artifact references.

## Recordkeeping rules

- Keep raw source records separate from summaries.
- Label each record's source, date, project, sensitivity, and verification status.
- Distinguish user-confirmed decisions from assistant suggestions and inferred conclusions.
- Record exact artifact paths, versions, hashes, and commits only when verified.
- Preserve historical records; mark superseded records rather than silently rewriting them.
- Do not assume a summary replaces original evidence.
- This repository is public. Do not commit private raw transcripts, personal data, credentials, API keys, or confidential material.

Use the templates in `../templates/` and metadata convention in `../schemas/ARCHIVE-METADATA-SCHEMA.md`.
