> Archived source reference, repackaged by Leotus-Richard on 2026-10-20. This is not an active skill or execution policy. Use the domain hub for current task scope and available capabilities; host commands, integrations, local-only rules, identity rules, and publishing steps below are historical examples. Modifications: discovery filename and local links normalized where needed, machine paths replaced where present; source substance retained.

---
name: typescript-best-practices
description: "Apply domain and type discipline to explicitly selected TypeScript work; not an always-active file matcher."
metadata:
  version: "1.0.0"
  profile: "local-task-toolkit"
  invocation: "task-specific"
  integration-status: "portable-instructions-host-untested"
---

# Typescript Best Practices

## Scope

Read `references/local-execution-contract.md` at task start. This skill is task-specific and local-only. Do not activate remote integrations, persistent modes, hooks or unrelated implementation.

## Workflow

1. Read the bundled syntax patterns and the type-system and boundary principles.
2. Derive types from authoritative schemas; model variants explicitly and brand primitives where interchange is unsafe.
3. Parse unknown external data at boundaries. Prefer total simple types and exhaustive handling to casts or optional-state bags.
4. Use the existing compiler/schema/test tools. Report diagnostics actually run; do not add a library merely to satisfy the reference.

## Default output

Type-safe local change or review with real compiler/test evidence.

## Failure boundary

Report the missing input or capability; do not fabricate evidence or broaden the task.

## Conditional skill dependencies

- `principle-type-system-discipline`: read the installed sibling skill only when its named discipline is required by the workflow.
- `principle-boundary-discipline`: read the installed sibling skill only when its named discipline is required by the workflow.

Use the host's actual skill loader, or read the current domain hub (historical dependency syntax removed) from this installed directory. Do not guess host tool names. Install the dependency closure shown in manifest.json if these siblings are absent.

## Upstream resources

The full original skill and its resources are preserved under `references/upstream/`. Read `references/upstream/ORIGINAL-SKILL.md` for detailed rubrics, templates and examples when its branch is relevant. Resolve its relative resource paths from that directory. Its tool names, model IDs, publication steps, transcript paths and persistent modes are source-specific examples, not permission to execute them. Follow this hub and the local execution contract when those instructions conflict.

## Provenance

Adapted from [pstack:typescript-best-practices](https://github.com/cursor/plugins/blob/1e5c90a4b6f249917bd21fe361b3a2a7deb741b8/pstack/skills/typescript-best-practices/SKILL.md). The original MIT notice is bundled. This is a local-only adaptation, not an endorsement or a claim of native host support.
