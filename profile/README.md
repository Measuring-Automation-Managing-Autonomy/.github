# MAMA — Measuring Automation & Measuring Autonomy

**MAMA** is an organization-backed, open framework and toolset that helps organizations plan, assess, govern, and improve investments in automation and autonomy — across projects involving AI and other technologies.

MAMA treats automation and autonomy as connected but **distinct** concerns:

- **Measuring automation** — what work and capabilities are automated, how well the automated process performs, what outcomes and benefits are realized, and what trade-offs and adverse effects appear.
- **Measuring autonomy** — what decision authority is delegated to people, teams, systems, networks, software, robots, or AI agents; within what scope; at what level; for how long; and under which controls and accountability.

MAMA integrates both views so leaders can manage their interplay — without collapsing them into one ladder or one scalar score.

## Naming: MAMA and `mama` are different things

> **First reference:** MAMA (Measuring Automation & Measuring Autonomy) uses the `mama` (measuring and managing autonomy) method for its autonomy-governance component.

| | **MAMA** (this organization) | **`mama`** (upstream method) |
|---|---|---|
| Expansion | Measuring Automation & Measuring Autonomy | measuring and managing autonomy |
| Role | Umbrella framework, architecture, shared toolset | One autonomy method used *within* MAMA |
| Canonical home | This organization | [`emmanuel-a-otchere/MeasuringAndManagingAutonomy`](https://github.com/emmanuel-a-otchere/MeasuringAndManagingAutonomy) |
| Current version | Framework & schema releases here | Ruleset v2.0.0, ledger schema 2 |
| Scale | Does not define one | L0 Submarine Line (no grant) through L1–L5; dimension scores 0–5; weakest link `min(D3, D4, D6)` |

The names are case-sensitive and their homes, ownership, repositories, and scores are not merged. MAMA consumes the `mama` tool's versioned outputs through an explicit interface; it never redefines, renames, or recalculates those scores. See [`mama-integrations`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-integrations) and the [integration contract](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/integration-contract.md).

## The traceability model

MAMA links, without collapsing:

**Organization/portfolio → investment/project → use case/process → technology/capability → automation activity + autonomy domain/decision rights → metrics/evidence/controls → outcomes and review decisions.**

A project may automate a process without delegating consequential decision rights. An autonomous unit may rely on both automated and human work. The [reference architecture](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/architecture.md) models both cases.

## Repositories

| Repository | Purpose | Status |
|---|---|---|
| [`mama-framework`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework) | Source of truth for what MAMA means: charter, glossary, reference architecture, lifecycle, templates, integration contract, external mappings | draft |
| [`mama-metrics`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-metrics) | Versioned metric taxonomy, metric-card schema, starter automation/value/impact metric library, baselining & attribution guidance | draft |
| [`mama-integrations`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-integrations) | Version-pinned import/export adapters connecting MAMA use cases to upstream `mama` ledgers and assessments; compatibility matrix | draft |
| [`mama-tools`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-tools) | Reference tooling: use-case registry, metric calculator, evidence record, portfolio view | planned — Phase 3 |
| [`mama-conformance`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-conformance) | Shared fixtures and conformance checks for schemas and integrations | planned — after interfaces stabilize |
| [`mama-examples`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-examples) | Synthetic case studies, worked end-to-end examples, sector profiles | planned — with pilots |
| [`mama-learning`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-learning) | Training modules, facilitator guides, adoption kits | optional, later |

Every artifact carries a public status label — `draft`, `pilot`, `reviewed`, `stable`, `deprecated`, or `archived` (see [GOVERNANCE.md](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/GOVERNANCE.md)). Phased delivery is tracked on the [MAMA Framework Roadmap](https://github.com/orgs/Measuring-Automation-Managing-Autonomy/projects/1) (CR MAMA-ORG-CR-001).

## Principles

1. **Two measures, never one score.** Automation performance/value measures and `mama` autonomy outputs stay separate, linked, and versioned. No composite MAMA score exists until its construct, weighting, and validity are established through research and governance.
2. **Evidence before claims.** A baseline and a defensible attribution method are required before claiming automation caused a benefit. Trade-offs and negative effects are reported alongside benefits.
3. **Context survives aggregation.** Cross-project comparisons disclose metric definitions, ruleset versions, scope, and data quality. No ranking rewards raw automation percentage or autonomy level.
4. **Autonomy ≠ safety.** A higher autonomy level is not inherently better or safer. Low guardrails, telemetry, or accountability are never averaged away.
5. **Open, versioned, evidence-linked decisions.** Core framework decisions are recorded, dissent is noted, and unresolved questions stay public.

## Governance

- [Charter & governance](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/charter.md) — stewardship council, groups, decision rights
- [Contribution guide](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/CONTRIBUTING.md)
- [Code of conduct](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/CODE_OF_CONDUCT.md)
- [Security policy](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/SECURITY.md)
- [License & IP policy](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/LICENSE-POLICY.md)
- [Support & contact](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/SUPPORT.md)

## Status & limitations

All public MAMA materials are **pilot-stage until the multi-organization pilot** (≥6 use cases, ≥3 organizations, ≥2 sectors) completes. MAMA provides no certification, regulatory approval, or proof of conformity, safety, or effectiveness. See the [charter's limitations section](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/charter.md#limitations).

## Contact

- General & proposals: open an issue in the relevant repository (see [SUPPORT.md](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/SUPPORT.md))
- Security: follow [SECURITY.md](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/SECURITY.md) — do not open public issues for vulnerabilities
- `mama` method itself: its maintainers, at [`emmanuel-a-otchere/MeasuringAndManagingAutonomy`](https://github.com/emmanuel-a-otchere/MeasuringAndManagingAutonomy)
