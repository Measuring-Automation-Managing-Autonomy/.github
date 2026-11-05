# Contributing to MAMA

**Status:** draft · Thanks for helping build MAMA (Measuring Automation, Managing Autonomy)!

This guide covers the whole organization. Each repository may add specifics in its own `CONTRIBUTING.md` or README.

## Ground rules

1. **Code of conduct** — everyone operates under the [Code of Conduct](CODE_OF_CONDUCT.md).
2. **Naming discipline is binding.** `MAMA` (uppercase) is the umbrella framework — *Measuring Automation, Managing Autonomy*. `` `mama` `` (lowercase, in code formatting) is the separate autonomy method — *measuring and managing autonomy*, owned at [`emmanuel-a-otchere/measuring-and-managing-autonomy`](https://github.com/emmanuel-a-otchere/measuring-and-managing-autonomy). Never merge the names, scores, or homes. First reference: *"MAMA (Measuring Automation, Managing Autonomy) uses the `mama` (measuring and managing autonomy) method for its autonomy-governance component."*
3. **Stay in your lane.** Proposals to change `mama` scoring, levels, or schema belong upstream. MAMA repos consume `mama` outputs; they never redefine them.
4. **No composite scores.** Don't propose aggregating automation metrics and autonomy outputs into a single score (see [ADR-003](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/decisions/adr-003-no-composite-score.md)).
5. **No sensitive data.** Issues, PRs, fixtures, and examples must contain only synthetic data. See the security policy for responsible disclosure.

## How work is organized

- **Proposals** use the issue templates: framework proposals and ADRs → `mama-framework`; metric proposals → `mama-metrics`; integration needs → `mama-integrations`.
- **Artifact status labels** (`draft` → `pilot` → `reviewed` → `stable`) are recorded in each repo's README table; changes to `reviewed`/`stable` artifacts require an ADR (see [GOVERNANCE.md](GOVERNANCE.md) §3–4).
- Every repository lists a named maintainer in its `MAINTAINERS.md`.

## Pull requests

- One logical change per PR; link the issue it resolves.
- Docs changes: update the artifact's status label and `CHANGELOG.md` if behavior/meaning changed.
- Code changes: add or update tests; CI must pass (tests, schema validation, lint where configured).
- Describe the evidence behind measurement claims — a metric card or guidance change should say what data or use informed it.
- Commits: short imperative subject lines (e.g., `metrics: add exception-rate card v0.2`).

## Versioning

- Schemas and metric libraries: semver; breaking changes need a migration note.
- The [compatibility matrix](https://github.com/Measuring-Automation-Managing-Autonomy/mama-integrations/blob/main/compatibility.md) declares which upstream `mama` ruleset/schema versions each MAMA release supports.

## Review & escalation

- Maintainers triage issues weekly; proposals sit open for comment for at least 7 days before an ADR is recorded.
- If a decision affects the core model, it goes to the [Stewardship Council process](GOVERNANCE.md#3-decision-rights). Dissent is recorded, and appeals follow [GOVERNANCE.md §3](GOVERNANCE.md#3-decision-rights).
