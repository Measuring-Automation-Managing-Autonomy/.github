# MAMA License & IP Policy

**Status:** draft · **Owned by:** MAMA Stewardship Council

## Licenses by content type

| Content | License | Rationale |
|---|---|---|
| Framework documents, charters, glossaries, guides, metric cards (prose & YAML definitions), schemas-as-specification | **CC-BY-4.0** | Definitions must be reusable with attribution across organizations, sectors, and publications |
| Executable code (adapters, validators, tools, CI scripts) | **Apache-2.0** | Permissive with an explicit patent grant; suitable for enterprise adoption |

Per repository:

| Repository | License |
|---|---|
| `.github` (governance & policy docs) | CC-BY-4.0 |
| `mama-framework` | CC-BY-4.0 |
| `mama-metrics` | CC-BY-4.0 (cards, schemas, docs); any code under `tools/` is Apache-2.0 |
| `mama-integrations` | Apache-2.0 |
| `mama-tools` (planned) | Apache-2.0 |
| `mama-examples` (planned) | CC-BY-4.0; bundled code Apache-2.0 |

Dual-licensed repositories state the split in their README and carry both license files where needed. Contributions are accepted under the repository's stated license(s) without additional terms.

## Relationship to the upstream `mama` method

The lowercase `mama` method (*measuring and managing autonomy*) is owned and maintained at [`emmanuel-a-otchere/measuring-and-managing-autonomy`](https://github.com/emmanuel-a-otchere/measuring-and-managing-autonomy) under its own license. MAMA:

- **consumes** its versioned outputs (assessments, ledgers) through documented interfaces;
- **does not fork, vendor, or reimplement** its scoring logic without an explicit maintainer agreement, compatible licensing, provenance records, and a compatibility plan (recorded as an ADR);
- **does not speak for it** — MAMA's descriptions of `mama` always point to the upstream repository as canonical.

## Attribution

When reusing MAMA definitions, attribute as: *"Definition from the MAMA framework (Measuring Automation, Managing Autonomy), `<repo>` v`<version>`, CC-BY-4.0."* Link the source file. Attribution for the `mama` method follows the upstream repository's terms.

## Naming & identity

"MAMA" (Measuring Automation, Managing Autonomy) and the lowercase `mama` method are distinct identities with distinct homes. Derivative works must not present themselves as the MAMA organization, imply the organization's endorsement, or merge the two names' scores or outputs. The case-sensitive naming rules in the [organization profile](profile/README.md) are binding.

## IP & provenance

- All contributions assert the contributor has the right to submit under the repository license.
- Any vendored third-party material must retain license notices, version identifiers, and a record of local changes.
- Worked examples and case studies use synthetic or explicitly approved, de-identified data only.
