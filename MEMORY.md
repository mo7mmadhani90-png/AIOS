# AIOS Memory

Status: Proposed v0.2 foundation

## Storage

Repository files are durable memory. Conversation details become durable only after being captured with their source and status.

| Knowledge | Canonical location |
| --- | --- |
| Identity and rules | SYSTEM.md and PROJECT_RULES.md |
| Execution process | AI_WORKFLOW.md |
| Current system next action | NEXT_TASK.md |
| System change history | CHANGELOG.md |
| Confirmed system defects | KNOWN_BUGS.md |
| System decisions | MEMORY/decisions/<id>.md |
| Project tasks and handoffs | PROJECTS/<project>/tasks/<id>.md |
| Project decisions | PROJECTS/<project>/decisions/<id>.md |
| Project research | PROJECTS/<project>/research/<id>.md |
| Project validation evidence | PROJECTS/<project>/qa/<task-id>.md |

Create record directories only when needed. IDs are unique within their directory. Use links to canonical records instead of copying mutable status into multiple places.

## Write and retrieval rules

Every new record includes author/role, date, project/task, source or revision, and status. Label facts, assumptions, proposals, and accepted decisions distinctly. Read current rules, task, accepted decisions, and relevant QA/bug records before resuming work. Check sources and revision freshness; resolve contradictory records through the decision process instead of silently choosing one.

Only the assigned writer edits a record. Preserve meaningful decision history with superseding records and Git history. Update task status after each handoff, and update CHANGELOG.md and NEXT_TASK.md with delivered system changes. Exclude credentials, tokens, unnecessary personal data, and raw sensitive logs; keep sanitized evidence or authorized references.

This is a file-based convention. Automatic retrieval, persistence hooks, access control, and retention enforcement remain future implementation work.
