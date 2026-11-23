# Upstream Contribution Guide

## Don't just fork it. Make it better. Send it upstream.

Open source works best when useful improvements travel back to the projects that need them. A fork can be a place to learn, test, repair, document, and collaborate—but the goal is not to collect copies. The goal is to help good work move forward.

**Discover → Fork → Improve → Verify → Submit upstream → Share**

A pull request is a proposal. The upstream maintainers decide whether to review, revise, accept, or decline it. Never describe a change as upstreamed until the upstream project has merged or otherwise formally incorporated it.

## 1. Discover before you fork

- Find the original project and confirm its canonical repository.
- Read its README, contribution guide, issue tracker, license, security policy, and code of conduct.
- Check whether the project is maintained and whether an issue or discussion already covers the problem.
- Prefer opening an issue or discussion before substantial work when the maintainers request it.
- Record the upstream URL, default branch, and exact base commit.

Do not assume that publicly visible source can be redistributed under any terms. If there is no clear license, treat reuse rights as unknown and ask the rights holder before copying or redistributing code.

## 2. Make a contribution station

A contribution station is a focused working space—often a fork—created to improve a specific upstream project.

Record:
- Original project URL and upstream owner.
- Fork URL, if one is created.
- Base branch and commit SHA.
- Why the station exists and the problem it aims to solve.
- Contributor or responsible team.
- Applicable license and any contribution terms (CLA, DCO, sign-off, or other requirements).
- Planned maintenance or handoff if the work remains independent.

Keep the upstream remote identifiable. Do not overwrite the upstream project's history or imply that the fork is the canonical source.

## 3. Improve in small, reviewable steps

- Keep changes focused on a clear problem.
- Preserve existing conventions and compatibility unless a deliberate change is justified.
- Add or update tests, documentation, examples, and migration notes as appropriate.
- Avoid bundling unrelated refactors into a fix.
- Never include credentials, private data, generated secrets, or material you do not have rights to contribute.
- Record important design decisions and known limitations.

## 4. Verify before proposing upstream

Before opening a pull request, record the checks actually performed:
- Tests and commands run, with results.
- Build, lint, type-check, or security checks where relevant.
- Supported environments and compatibility impact.
- Known failures, untested paths, and remaining risks.

Do not claim tests passed if they were not run. Include reproducible steps and evidence that maintainers can inspect.

## 5. Submit upstream respectfully

- Follow the upstream project's contribution instructions exactly.
- Link the relevant issue or discussion.
- Explain the problem, the chosen solution, alternatives considered, and user impact.
- Include test evidence and screenshots only when useful.
- Sign a CLA, DCO, or other agreement only after understanding its terms and having authority to do so.
- Respond constructively to review and revise the patch when appropriate.

Upstream maintainers retain control over their project and its acceptance decisions. A submitted PR is not an endorsement, merge, or transfer of ownership.

## 6. Track the outcome

Record the PR or patch URL and its status: draft, open, changes requested, accepted/merged, declined, closed, or withdrawn. Include the date and relevant upstream commit when merged.

If a proposal is declined or the project is inactive:
- Record the outcome accurately.
- Do not pressure maintainers or repeatedly submit unchanged work.
- Decide whether the independent fork has a legitimate maintenance purpose.
- Keep attribution, license notices, and clear divergence notes.
- Make it easy for users to distinguish upstream behavior from fork-only changes.

Independent work can still be useful, but it must not be represented as accepted upstream work.

## 7. Share what others can build upon

Publish a concise contribution record with:
- Original upstream project and license.
- Contribution station/fork URL.
- Problem and improvement summary.
- Base and resulting commit references.
- Verification evidence and limitations.
- Pull request link and current outcome.
- Maintenance owner and next steps.

Where practical, upstream reusable fixes rather than maintaining permanent patches in isolation. Where upstreaming is not appropriate, document why and maintain the work transparently.

## Contribution station lifecycle

| Stage | Required record |
|---|---|
| Discover | Canonical project URL, license, project health |
| Fork | Fork URL, base branch and commit, reason |
| Improve | Objective, change summary, responsible contributor |
| Verify | Tests, evidence, limitations |
| Submit | PR/patch URL, upstream instructions followed |
| Share | Outcome, attribution, maintenance plan |

## Start here

- [Submit an upstream contribution record](../../issues/new?template=upstream-contribution.yml)
- [Submit a public material deposit](../../issues/new?template=public-material-deposit.yml)
- [Review the ecosystem build](./HUFFMAN-ECOSYSTEM.md)
- [Review the build roadmap](./BUILD-ROADMAP.md)

**We are not here to collect forks. We are here to make open-source work more useful, more connected, and more durable.**

One improvement can help one project. Shared improvements can strengthen an ecosystem. Build what others can build upon.
