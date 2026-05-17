# Operating Model

## Team Topology

| Group | Ownership |
| --- | --- |
| Executive sponsor | Business priority, funding, and scale decisions |
| Delivery lead | Roadmap, stakeholder alignment, dependency management |
| AI platform owner | Shared tooling, access, deployment patterns, observability |
| Product/workflow owner | Workflow definition, acceptance criteria, user adoption |
| Engineering pod | Implementation, integrations, test harnesses, runbooks |
| Risk and governance partner | Data handling, human-review boundaries, audit evidence |

## Delivery Flow

1. Intake: identify workflow, pain, volume, risk, and current baseline.
2. Triage: score for value, feasibility, data readiness, and safety.
3. Pilot: build the smallest version that can produce measurable workflow output.
4. Evaluate: compare quality, cycle time, rework, user trust, and unsafe-action attempts.
5. Harden: add monitoring, runbooks, access controls, and rollback.
6. Scale: onboard the next team only after the first workflow has operational ownership.

## Platform Decision Matrix

| Criterion | Why it matters | Decision signal |
| --- | --- | --- |
| Data residency | TELUS/client data may have strict handling needs | Region controls and auditability |
| Tool integration | Agents need safe access to systems of work | Permission model and connector maturity |
| Evaluation support | Quality must be measurable over time | Trace, eval, and feedback-loop support |
| Observability | Delivery leaders need operational signal | Logs, metrics, failed-action visibility |
| Cost control | Scale can become expensive quickly | Token, compute, and workflow-level cost reporting |
| Human review | Risky actions need approvals | Native approval gates or easy workflow integration |
