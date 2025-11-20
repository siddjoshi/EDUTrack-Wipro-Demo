---
description: 'Convert approved requirements into a delivery-ready backlog hierarchy with clear traceability, sequencing guidance, and execution readiness notes.'
tools: []
---
# Phase 2.3 – Product Operations Prompt (Backlog Decomposition & Delivery Readiness)

## Role Mission
Convert approved requirements into a delivery-ready backlog hierarchy with clear traceability, sequencing guidance, and execution readiness notes.

## Inputs & References
| Source | Location | Purpose |
|--------|----------|---------|
| BRD | `docs/requirements/BRD.md` | Confirm business objectives, KPIs, stakeholders. |
| PRD | `docs/requirements/PRD.md` | Use feature catalogue, personas, acceptance criteria. |
| SRS | `docs/requirements/SRS.md` | Align functional detail and integration needs. |
| RTM | `docs/requirements/RTM.md` | Ensure traceability and identify gaps. |
| Governance artefacts | `docs/inception/stakeholder-register.md`, `docs/inception/communication-plan.md` | Assign ownership, cadence, approvals for backlog reviews. |
| Change Log | `docs/change-log.md` | Capture existing decisions, questions, risks. |
| Templates | ` templates/EPIC.md`, ` templates/Feature.md`, ` templates/Story.md`, ` templates/Task.md` | Provide structure and mandatory metadata for backlog artefacts. |

## Expected Outputs
| Artefact | Destination | Format | Notes |
|----------|-------------|--------|-------|
| Epics | `backlog/epics/EP-xxxx.md` | Markdown | Clone template for each capability; maintain document control and approvals. |
| Features | `backlog/features/FE-xxxx.md` | Markdown | Map to epics and requirement IDs. |
| Stories | `backlog/stories/US-xxxx.md` | Markdown | Include acceptance criteria, NFR callouts, DoR/DoD. |
| Tasks | `backlog/tasks/TSK-xxxx.md` | Markdown | Detail implementation activities, test expectations. |
| RTM Update | `docs/requirements/RTM.md` | Markdown | Link backlog IDs to originating requirements and planned tests/design artefacts. |
| Change Log Update | `docs/change-log.md` | Markdown | Record backlog baseline, risks, and follow-up actions. |

## Procedure
1. **Scope Confirmation** – Review BRD/PRD/SRS priorities with Product Manager and Systems Analyst; capture dependencies, constraints, NFR drivers.
2. **Create Epics** – For each major capability, clone ` templates/EPIC.md` into `backlog/epics/`; populate metadata, scope, traceability, success metrics, dependencies, risks, approvals.
3. **Decompose into Features** – Use ` templates/Feature.md` for each epic; document user value, functional slices, dependencies, non-functional considerations, release/rollout strategy.
4. **Author Stories** – Generate story files from ` templates/Story.md`; include user narrative, acceptance criteria (Gherkin), NFR hooks, analytics, dependencies, DoR/DoD checklists.
5. **Detail Tasks** – Break each story into tasks using ` templates/Task.md`; specify activities, deliverables, validation evidence, traceability, approvals.
6. **Maintain Traceability** – Update each artefact with BRD/PRD/SRS references and backlog IDs; refresh `docs/requirements/RTM.md` to include backlog mappings and planned validation.
7. **Document Parallelisation Guidance** – Note sequencing, dependencies between features/stories, NFR considerations, and recommended sprint allocation.
8. **Update Change Log** – Log backlog baseline, RTM updates, outstanding items, and owners with due dates.
9. **Ensure Versioning** – Populate document control, change log, and approvals sections in every backlog artefact.

## Traceability & Governance
- Guarantee every backlog item references originating requirement IDs and planned validation artefacts.
- Share parallelisation and dependency notes with Engineering Lead and QA Lead.
- Flag open questions or risks for change log tracking and stakeholder follow-up.

## Completion Checklist
- [ ] Epic/Feature/Story/Task artefacts created without placeholders and stored in respective directories.
- [ ] RTM updated with forward links from requirements to backlog and assigned owners.
- [ ] Parallelisation guidance and dependencies documented for delivery planning.
- [ ] Change log updated with backlog baseline, risks, and pending actions.

## Parallelisation Notes
Engineering (Phase 4.1/4.2) and QA planning (Phase 5) can start after backlog baseline; maintain alignment through RTM and change log updates.
```
