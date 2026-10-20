> Archived source reference, repackaged by Leotus-Richard on 2026-10-20. This is not an active skill or execution policy. Use the domain hub for current task scope and available capabilities; host commands, integrations, local-only rules, identity rules, and publishing steps below are historical examples. Modifications: discovery filename and local links normalized where needed, machine paths replaced where present; source substance retained.

---
name: codebase-design
description: "Choose deep module interfaces, domain ownership and public test seams; not a mandatory architecture session."
metadata:
  version: "1.0.0"
  profile: "local-task-toolkit"
  invocation: "task-specific"
  integration-status: "portable-instructions-host-untested"
---

# Codebase Design

## Scope

Read `references/local-execution-contract.md` at task start. This skill is task-specific and local-only. Do not activate remote integrations, persistent modes, hooks or unrelated implementation.

## Workflow

1. Read the source vocabulary and optional deepening/alternative-interface references when the relevant question arises.
2. Trace caller usage and the knowledge the module should own.
3. Compare interface depth, meaningful hidden complexity, locality, leverage and seam placement.
4. Prefer a small coherent interface; do not invent a layer that merely passes through the same methods.

## Default output

Interface/seam recommendation with alternatives and owned invariants.

## Failure boundary

Report the missing input or capability; do not fabricate evidence or broaden the task.

## Upstream resources

The full original skill and its resources are preserved under `references/upstream/`. Read `references/upstream/ORIGINAL-SKILL.md` for detailed rubrics, templates and examples when its branch is relevant. Resolve its relative resource paths from that directory. Its tool names, model IDs, publication steps, transcript paths and persistent modes are source-specific examples, not permission to execute them. Follow this hub and the local execution contract when those instructions conflict.

## Provenance

Adapted from [mattpocock:codebase-design](https://github.com/mattpocock/skills/blob/49dd158d1076134a641b33efb035946536778336/skills/engineering/codebase-design/SKILL.md). The original MIT notice is bundled. This is a local-only adaptation, not an endorsement or a claim of native host support.
