# AIOS WORKFLOW

Version: 0.1.0

## Official Workflow

All development follows this cycle:

1. Extract facts and decisions from discussions.
2. Update the correct repository file.
3. Update CHANGELOG.md.
4. Update NEXT_TASK.md.
5. Move to the next approved phase.

## Source of Truth

The repository is the official source of project knowledge.

Conversation history is not considered permanent memory unless recorded in repository files.

## Execution Cycle

Goal → Planning → Execution → Internal QA → Documentation → Delivery

## Quality Gate

No task is considered complete until:

- Result is validated.
- Known issues are documented.
- Next action is defined.

## Proposed v0.2 Agent Mapping

Use [AGENTS/README.md](AGENTS/README.md) for task states and handoff fields. CEO_AGENT confirms direction within Owner authority; PROJECT_MANAGER plans; ARCHITECT_AGENT designs and RESEARCH_AGENT supplies evidence when needed; WORKER_AGENT executes; QA_AGENT validates; CEO_AGENT accepts delivery after the quality gate. Record decisions and evidence using [DECISIONS.md](DECISIONS.md) and [MEMORY.md](MEMORY.md).

This mapping is a review proposal. The foundation does not launch agents or enforce tool permissions.
