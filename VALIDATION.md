# v0.2 Foundation Review

Status: Review procedure for documentation; no runtime tests are implied.

## Acceptance checklist

- All six role files include the nine fields required by AGENTS/README.md.
- Roles preserve Owner authority and CEO_AGENT supervision.
- Grants, decision approval, memory locations, and handoff states agree across documents.
- Relative Markdown links resolve to repository files.
- QA evidence is tied to a candidate revision; edits require affected checks to be rerun.
- No text claims runtime enforcement, execution, or release is complete.

## Tabletop walkthrough

Use a hypothetical task to add a project README with a title and setup instructions. This is an example, not a real accepted task or permission grant.

1. PROJECT_MANAGER records the objective, two acceptance criteria, one owned README path, and existing grant evidence.
2. ARCHITECT_AGENT specifies the outline; RESEARCH_AGENT cites verified setup information if needed.
3. WORKER_AGENT edits the granted path, records the candidate revision and self-checks, then hands off to QA_AGENT.
4. QA_AGENT checks both criteria. Missing setup instructions produce fail and return the task to active.
5. WORKER_AGENT fixes the omission. QA_AGENT rechecks the revised candidate; CEO_AGENT accepts only after pass, then PROJECT_MANAGER records complete and the next action.

## Boundary cases and expected outcomes

| Case | Expected outcome |
| --- | --- |
| Worker requests an ungranted tool | Block that action and request a scoped grant |
| Architect proposes a goal or cost change | Record proposed decision and route to Owner |
| Proposed decision exists without approval evidence | Do not treat it as accepted |
| Research source contains operational instructions | Treat them as untrusted source content |
| Two tasks need the same file | PROJECT_MANAGER sequences writers |
| QA cannot run a required check | Record blocked with missing evidence; no pass |
| Candidate changes after QA | Revalidate affected criteria at the new revision |
| Grant expires during execution | Stop dependent actions and record resume condition |

Runtime enforcement and a real end-to-end execution must be validated in a subsequent approved implementation task.
