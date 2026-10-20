> Archived source reference, repackaged by Leotus-Richard on 2026-10-20. This is not an active skill or execution policy. Use the domain hub for current task scope and available capabilities; host commands, integrations, local-only rules, identity rules, and publishing steps below are historical examples. Modifications: discovery filename and local links normalized where needed, machine paths replaced where present; source substance retained.

---
name: domain-modeling
description: "Define or refine domain terminology, invariants, glossaries and architectural decisions; not merely explain existing code."
metadata:
  version: "1.0.0"
  profile: "local-task-toolkit"
  invocation: "task-specific"
  integration-status: "portable-instructions-host-untested"
---

# Domain Modeling

## Scope

Read `references/local-execution-contract.md` at task start. This skill is task-specific and local-only. Do not activate remote integrations, persistent modes, hooks or unrelated implementation.

## Workflow

1. Locate the glossary/context map and relevant ADRs. Use the bundled glossary and ADR formats.
2. Resolve overloaded terminology with concrete scenarios. Separate domain meaning from implementation details.
3. Check the local code against stated domain rules and surface contradictions rather than silently choosing.
4. Capture resolved terms immediately when editing is authorized. Propose unresolved changes rather than inventing agreement.
5. Write an ADR only for a hard-to-reverse, surprising decision with real alternatives.

## Default output

Resolved glossary terms, invariants, contradictions, and warranted ADRs.

## Failure boundary

Report the missing input or capability; do not fabricate evidence or broaden the task.

## Upstream resources

The full original skill and its resources are preserved under `references/upstream/`. Read `references/upstream/ORIGINAL-SKILL.md` for detailed rubrics, templates and examples when its branch is relevant. Resolve its relative resource paths from that directory. Its tool names, model IDs, publication steps, transcript paths and persistent modes are source-specific examples, not permission to execute them. Follow this hub and the local execution contract when those instructions conflict.

## Provenance

Adapted from [mattpocock:domain-modeling](https://github.com/mattpocock/skills/blob/49dd158d1076134a641b33efb035946536778336/skills/engineering/domain-modeling/SKILL.md). The original MIT notice is bundled. This is a local-only adaptation, not an endorsement or a claim of native host support.
