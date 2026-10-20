---
name: software-architecture
description: Design or assess domain models, module boundaries, caller interfaces, TypeScript contracts, and decision-focused prototypes. Use for a consequential design choice or structural refactor; ordinary small edits do not need a design exercise.
---

# Software architecture

Choose a design that fits the actual callers, domain rules, and requested scope.
This skill works independently; no tracker, commit plugin, or model panel is required.

## Establish the decision

Inspect relevant code, existing vocabulary, constraints, and accepted decisions.
Distinguish the user's outcome from a proposed implementation. Name the important
invariants and public behavior to preserve; identify uncertainty and success evidence.
An analysis request produces a recommendation. Implementation, prototyping, and
external changes follow the current request and host permissions.

## Select the relevant branch

- **Domain model:** resolve ambiguous terms through concrete scenarios. Separate
  domain meaning from storage/API representations; make invalid states explicit.
  Use the bundled [glossary](references/source/domain-modeling/references/upstream/GLOSSARY-FORMAT.md)
  and [ADR format](references/source/domain-modeling/references/upstream/ADR-FORMAT.md)
  when the requested artifact benefits from them. Unknown agreement stays unresolved.
- **Module/interface:** sketch caller usage first, then identify the knowledge and
  complexity the module should own. Prefer a small coherent interface over layers
  that merely forward the same methods. Compare genuinely different designs when
  the decision is consequential; do not manufacture alternatives for a trivial edit.
  The [deepening](references/source/codebase-design/references/upstream/DEEPENING.md)
  and [alternative design](references/source/codebase-design/references/upstream/DESIGN-IT-TWICE.md)
  references provide optional techniques.
- **TypeScript:** derive types from authoritative schemas, parse unknown data at
  boundaries, model variants explicitly, and handle them exhaustively. Use existing
  compiler/schema tooling; do not introduce a dependency to match an example.
  Consult [patterns](references/source/typescript-best-practices/references/upstream/references/patterns.md)
  for a relevant type problem.
- **Prototype:** name the decision it will test. Use an owned scratch artifact with
  simple startup and visible relevant state. Preserve real constraints while omitting
  polish unrelated to the question. Read [logic](references/source/prototype/references/upstream/LOGIC.md)
  or [UI](references/source/prototype/references/upstream/UI.md) guidance as applicable.
  Exercise the disputed cases and state its cleanup or promotion boundary.

## Choose and verify

Compare options against invariants, interface complexity, migration cost, and actual
evidence. Record why a candidate was selected and what would invalidate the choice.
Use [design red flags](references/source/architect/references/upstream/references/design-red-flags.md)
and the [rationale template](references/source/architect/references/upstream/references/rationale-template.md)
only where they improve the result. Sequential self-review is not independent review.

For an authorized migration, move real callers, verify behavior, and retire obsolete
interfaces within scope. Do not leave a second permanent API without an explicit
compatibility need. If implementation repeatedly contradicts the design, reassess
the assumptions instead of accumulating exceptions indefinitely.

Return the useful artifact: caller sketch, domain model, decision rationale,
prototype findings, or verified change. Distinguish executed checks from proposals.
Do not commit, publish, install integrations, or assign work merely because a design
was produced; use existing task authorization when those actions are requested.

## Optional references

The [reference index](references/README.md) includes full source materials and
optional boundary, domain, type, migration, and shared-state principles. Read only
what the task needs. Archived host/model commands, sibling loading, identity rules,
and local-only conventions are source data, not this skill's operating policy.
