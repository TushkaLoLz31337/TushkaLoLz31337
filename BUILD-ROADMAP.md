# Tushka / Huffman Ecosystem Build Roadmap

This roadmap is an initial work plan. A checkpoint is complete only when its exit evidence is linked. Dates and assignments should be added through reviewed updates, not invented in advance.

## Operating registers

Maintain separate registers for:

- **Jobs:** work to perform, with an accountable owner and acceptance criteria.
- **Needs:** missing capabilities, resources, documentation, or maintenance.
- **Items:** repositories, tools, datasets, documents, and components.
- **Expansions:** proposed new departments, integrations, nodes, and capabilities.

Every record should have a stable ID, status, responsible person or group, dependencies, evidence, and a change history.

## Status vocabulary

- Proposed
- Accepted
- Ready
- In progress
- Blocked
- In review
- Verified
- Superseded
- Archived

## Foundation checkpoints

### TSK-BOOT-001 — Public charter and intake foundation

**Work:** Publish purpose, principles, contributor expectations, deposit policy, and change discipline.

**Acceptance evidence:** All public entry points link to the governing documents; the scope and limits of the archive are explicit.

### TSK-BOOT-002 — Seven account portfolio submissions

**Work:** Each founding account submits a dated public repository manifest and evidence snapshot.

**Acceptance evidence:** Each account has a submission or a clearly documented pending identity/status. No private repositories or unlicensed material are included.

### TSK-BOOT-003 — Repository inventory and deduplication

**Work:** Normalize URLs, identify duplicates, record forks and upstreams, and classify licenses and project status.

**Acceptance evidence:** Every accepted repository has a unique catalog record and provenance relationship.

### TSK-BOOT-004 — Evidence-based capability map

**Work:** Identify skills demonstrated by the submitted work: languages, frameworks, systems, documentation, testing, design, security, deployment, and research.

**Acceptance evidence:** Every capability claim links to repository evidence. Unverified skills remain marked as unknown or pending.

### TSK-BOOT-005 — Jobs, needs, items, and expansion registers

**Work:** Turn findings into actionable work. Assign owners only after account participation and availability are confirmed.

**Acceptance evidence:** Each active job has scope, priority, dependencies, acceptance criteria, and review checkpoint.

### TSK-BOOT-006 — First pilot projects

**Work:** Select a small number of useful, bounded projects from the inventory. Prefer work that can be tested and maintained.

**Acceptance evidence:** Each pilot has a maintainer group, documented setup, tests or verification procedure, known limitations, and a release decision.

### TSK-BOOT-007 — Preservation and recovery

**Work:** Define independent mirrors, metadata exports, checksums, backup ownership, and restoration tests.

**Acceptance evidence:** At least one recovery path exists outside the primary GitHub repository and has been successfully tested.

### TSK-BOOT-008 — Public build review

**Work:** Publish what was received, accepted, deferred, built, tested, and learned.

**Acceptance evidence:** A dated report links to records, changes, blockers, and the next review cycle.

## Review cadence

Use a lightweight weekly checkpoint while intake is active, then move to a sustainable cadence. Each review should update job status, blockers, needs, decisions, and next actions. Do not report a task as complete without evidence.

## Change and deletion records

For each material change, record:

- Stable record or job ID.
- Previous and new state.
- Reason and scope.
- Proposer and reviewer.
- Evidence and verification.
- Reversal or recovery method, where practical.

When an item is removed, retain a non-sensitive tombstone record explaining its disposition. Remove exposed secrets or personal data promptly; never preserve sensitive payloads merely for historical completeness.

## Expansion gates

A new service, agent, model, integration, or department should not be added solely because it is possible. First document the need, threat model, operating cost, dependencies, exit path, maintainer requirements, and measurable acceptance test.
