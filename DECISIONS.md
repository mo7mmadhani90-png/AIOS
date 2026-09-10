# AIOS Decisions

Status: Proposed v0.2 foundation

## Lifecycle

Record decisions as proposed, accepted, rejected, or superseded. Writing a proposal does not approve it. An accepted record requires an authorized decision maker, approval evidence, and storage in the repository. Preserve prior records when superseding them and link the replacement.

Routine choices within assigned permissions may be accepted by the responsible role. CEO_AGENT resolves coordination conflicts within the approved objective. Conditions in [PROJECT_RULES.md](PROJECT_RULES.md), including changes to goals, costs/resources, or final results, go to the Owner through CEO_AGENT. Pause dependent execution while approval or essential information is missing.

## Record format

- ID, date, project/task, and author.
- Question, context, and source references.
- Options, recommendation, consequences, and affected acceptance criteria.
- Required authority and status.
- Decision maker and approval evidence; leave empty while proposed.
- Affected files, follow-up owner, and supersedes/superseded-by references.

Store project decisions under PROJECTS/<project>/decisions/. System-wide records belong under MEMORY/decisions/. Create folders when the first real record exists. Proposed records may be reviewed on a branch; acceptance must cite actual approval and does not itself authorize merging or deployment.

## Foundation proposal

The six roles and shared contracts in this change are proposed for v0.2 review. Authorization to prepare this proposal is not approval of every proposed policy or a released v0.2 runtime. Record the review outcome before treating the proposal as accepted.
