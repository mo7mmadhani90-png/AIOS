# AIOS Agents

Status: Proposed v0.2 foundation; documentation only, with no agent runtime or automatic tool enforcement.

## Roles

All agents operate under CEO_AGENT supervision; CEO_AGENT remains accountable to the Owner.

| Role | Responsibility |
| --- | --- |
| [CEO_AGENT](CEO_AGENT.md) | Keep execution aligned with the Owner-approved objective. |
| [PROJECT_MANAGER](PROJECT_MANAGER.md) | Turn the approved objective into traceable tasks. |
| [ARCHITECT_AGENT](ARCHITECT_AGENT.md) | Define a design that satisfies the approved requirements. |
| [RESEARCH_AGENT](RESEARCH_AGENT.md) | Provide evidence for project decisions. |
| [QA_AGENT](QA_AGENT.md) | Verify the result against the task's acceptance criteria. |
| [WORKER_AGENT](WORKER_AGENT.md) | Implement one assigned task within its boundaries. |

Each role defines Goal, Responsibilities, Permissions, Inputs, Outputs, Allowed tools, Decision rules, Success criteria, and Delivery standards.

## Shared contracts

Read [SYSTEM.md](../SYSTEM.md), [PROJECT_RULES.md](../PROJECT_RULES.md), and [AI_WORKFLOW.md](../AI_WORKFLOW.md) first. [PERMISSIONS.md](../PERMISSIONS.md), [DECISIONS.md](../DECISIONS.md), and [MEMORY.md](../MEMORY.md) make those rules operational without overriding them. Conflicts are recorded and routed to CEO_AGENT; Owner authority remains unchanged.

## Task and handoff contract

PROJECT_MANAGER creates a task record before execution. Required fields:

- ID and approved objective reference.
- Scope, excluded work, acceptance criteria, and constraints.
- Assigned role, owned paths, allowed tools/actions, and grant evidence.
- Dependencies and input revision.
- Status: planned, active, blocked, in_qa, or complete.
- Outputs, candidate revision, validation evidence, unresolved issues, and next owner/action.

Planned tasks become active only when inputs and permissions are available. A worker submits active work to in_qa with self-check evidence. QA failure returns it to active with concrete findings; missing dependencies set it to blocked with a resume condition. QA pass plus CEO_AGENT acceptance permits complete. Any edit after QA requires revalidation of affected criteria at the new revision.

Handoffs use the same task record rather than duplicating state. Assign one writer per path at a time. Conflicting edits return to PROJECT_MANAGER for sequencing. QA is a distinct review step from worker self-checks; if one operator performs both roles, record that limitation.

See [the review walkthrough](../VALIDATION.md) before accepting the foundation.
