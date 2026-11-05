# MAMA Governance

**Status:** draft · **Applies to:** every repository, schema, tool, and published asset in this organization · **Owned by:** MAMA Stewardship Council

This document defines how MAMA (Measuring Automation, Managing Autonomy) is stewarded. The canonical charter lives in [`mama-framework/charter.md`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/charter.md); this file is the organization-level operating agreement.

## 1. Stewardship Council

The MAMA Stewardship Council owns the charter, identity, principles, architecture, release policy, public claims, risk posture, and priorities. It must include these perspectives, each held by a named person:

| Perspective | Holder |
|---|---|
| Operations / business | *vacant — see issues in this repo* |
| Automation & AI engineering | *vacant* |
| Workforce / people | *vacant* |
| Security / risk | *vacant* |
| Research / measurement | *vacant* |
| Affected stakeholders | *vacant* |

Initial council formation is tracked in [`mama-framework/MAINTAINERS.md`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/MAINTAINERS.md). Until the council is fully seated, decisions default to the repository maintainers with public records and a 7-day comment window before taking effect.

## 2. Working groups

| Group | Owns | Home |
|---|---|---|
| Framework & Interoperability | Core concepts, system/use-case model, metric taxonomy, schemas, crosswalks; coordinates with `mama` maintainers on the autonomy interface | `mama-framework` |
| Automation Measurement & Value | Metric cards, baselining/attribution methods, operational indicators, impact measures | `mama-metrics` |
| Tools & Platform | MAMA-owned tools, integrations, dashboards, accessibility, CI/release, documentation tooling, security | `mama-tools` (Phase 3) |
| Validation & Research | Pilots, research ethics, inter-rater checks, outcome validation, external review | `mama-framework` / `mama-examples` |
| Adoption & Education | Playbooks, training, facilitator guides, sector starter kits | `mama-learning` (optional, later) |
| Sector Working Groups | Context-specific profiles and examples without silently changing the core model | proposed in issues |

## 3. Decision rights

| Decision | Decided by | Record |
|---|---|---|
| Charter, principles, architecture | Stewardship Council | ADR in `mama-framework/decisions/` |
| Metric definitions & schema | Automation Measurement & Value Group | ADR + schema version bump |
| `mama` interface & compatibility | Framework & Interoperability Group, with `mama` maintainers consulted | ADR + `mama-integrations/compatibility.md` |
| Tool releases | Tools & Platform Group maintainer | Release notes + CHANGELOG |
| New repositories or retirement | Stewardship Council | ADR |
| Sector profiles | Sector Working Group + framework Group review | Profile doc with applicability notes |

Rules:

- Core framework decisions are **open, versioned, and evidence-linked**. Every ADR states context, options, decision, consequences, and dissent.
- **Dissent and unresolved questions are recorded**, not suppressed.
- Tool vendors, assessment subjects, independent evaluators, and method stewards are kept in **separate roles** where conflicts could compromise credibility. Declared conflicts of interest are listed in `MAINTAINERS.md`.
- Decisions may be appealed by opening an issue against the ADR; the council responds within 14 days and records the outcome either way.

## 4. Artifact status labels

Every public framework/tool asset carries exactly one status, stated in its README and frontmatter, and is listed with a named maintainer:

| Label | Meaning |
|---|---|
| `draft` | Under active development; may change without notice; not for conformance claims |
| `pilot` | In structured use with pilot organizations; feedback-driven changes |
| `reviewed` | Passed internal/external review; changes require an ADR |
| `stable` | Versioned compatibility guarantees; deprecation policy applies |
| `deprecated` | Replaced or withdrawn; kept for migration guidance only |
| `archived` | Read-only historical record |

## 5. Release governance

- Schemas and metric libraries use semantic versioning with migration notes for any breaking change.
- Compatibility with upstream `mama` is declared per release in `mama-integrations/compatibility.md`; unknown upstream ruleset/schema versions fail safely with a clear warning.
- Releases list known limitations. Reproducible checks (tests, schema validation, conformance fixtures) run in CI before release.

## 6. Public claims

- No artifact may claim certification, regulatory approval, universal validity, or endorsement by any external body (NIST, ISO, OECD, TM Forum, OWASP, MITRE, or others). External mappings document scope, gaps, versions, and limitations — see [`mama-framework/external-mappings.md`](https://github.com/Measuring-Automation-Managing-Autonomy/mama-framework/blob/main/external-mappings.md).
- MAMA and the lowercase `mama` method are never merged in claims, scores, or identity. The naming rules in the [organization profile](https://github.com/Measuring-Automation-Managing-Autonomy/.github/blob/main/profile/README.md) are binding on all published material.

## 7. Data handling

Pilot and contributor data follow the privacy/data policy: data minimization, informed permission, local-first options, retention limits, and redaction. Test data in public repos must be synthetic — never real customer or sensitive pilot data.
