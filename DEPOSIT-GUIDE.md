# Public Material Deposit Guide

This guide explains how a participating account submits public open-source material to the Tushka / Huffman Ecosystem public build.

## Scope and safety

Submit only material that is already public and that you have the right to identify and describe. A public GitHub repository is not automatically licensed for arbitrary redistribution. Do not upload secrets, access tokens, private messages, personal information, private repository contents, or third-party material whose license does not permit the proposed use.

The initial deposit is a **catalog and evidence snapshot**. It does not require a fork or a source-code copy.

## Before submitting

For each repository, collect:

- Canonical repository URL and repository name.
- Account submitting the record.
- Snapshot date (UTC) and default branch.
- Commit SHA identifying the snapshot where available.
- Short description and primary purpose.
- Original / fork / mirror / derivative classification.
- Upstream repository URL, if applicable.
- License identifier and license file location; use `NOASSERTION` if not yet verified.
- Languages and relevant technologies, where known.
- Current status: working, prototype, research, archived, or unknown.
- Demonstrated capabilities, supported by links to code, documentation, releases, tests, or demos.
- Known limitations, security concerns, and maintenance needs.
- Whether collaboration is invited and what help is needed.

## Submission steps

1. Use the **Public material deposit** issue template.
2. Submit one request per account snapshot. For large portfolios, attach or link a CSV/JSON manifest rather than pasting hundreds of entries into the issue.
3. Include a date and a stable commit reference for each repository where practical.
4. Mark forks and identify upstream projects. Do not present upstream work as original work.
5. State the license accurately. If uncertain, mark it unknown; do not guess.
6. List any repositories that should be excluded from intake and explain why.
7. Submit and wait for intake review.

## Review and acceptance

Reviewers check:

- The repository is public and reachable.
- The submitting account is correctly identified.
- Duplicate canonical URLs are consolidated.
- Original/fork/upstream relationships are represented accurately.
- License and redistribution limits are respected.
- Snapshot references are reproducible where possible.
- Secrets and personal data are not being exposed.
- The claimed capability is supported by evidence.
- The record has a clear status and next action.

A request may be accepted, returned for clarification, partially accepted, or declined. A rejected or withdrawn submission should retain a short, non-sensitive decision record.

## What happens after acceptance

The catalog receives a stable record ID. The archive links to the source repository and records the snapshot metadata. Source mirroring, Git bundles, or other preservation copies are separate decisions requiring a documented reason, license review, and storage/recovery plan.

## Suggested manifest fields

```json
{
  "schema_version": "1.0",
  "contributor_account": "GitHub login",
  "snapshot_date_utc": "YYYY-MM-DD",
  "repositories": [
    {
      "record_id": "TUSHKA-ITEM-0001",
      "url": "https://github.com/OWNER/REPOSITORY",
      "snapshot_commit": "full commit SHA",
      "default_branch": "main",
      "relationship": "original | fork | mirror | derivative | unknown",
      "upstream_url": null,
      "license": "SPDX identifier or NOASSERTION",
      "status": "working | prototype | research | archived | unknown",
      "purpose": "Short factual description",
      "capabilities": [],
      "evidence": [],
      "limitations": [],
      "needs": []
    }
  ]
}
```

Do not include credentials or private information in a manifest.

## Snapshot quality

A screenshot alone is not a sufficient technical snapshot. Prefer a repository URL plus commit SHA, README and license references, release/test evidence, and a generated manifest. Screenshots may supplement but should not replace inspectable source references.

## Provenance rule

The source repository remains the authoritative origin unless its maintainers state otherwise. Cataloging does not transfer copyright, ownership, maintainer authority, or project identity.
