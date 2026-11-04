# Definition of Ready and Definition of Done

## Definition of Ready (per backlog item)

An item can enter a sprint when all of these are true:

- [ ] Written as a user-visible outcome: who wants it, what they get, why
- [ ] Acceptance criteria are testable and agreed with the Product Owner
- [ ] Dependencies identified; any external team has acknowledged the date
- [ ] Design or technical approach sketched, if the work is not routine
- [ ] Fits in roughly half a sprint; otherwise split it (`story-splitting.md`)
- [ ] No open question that only a stakeholder can answer

**Guard rail:** if applying DoR takes more than two minutes per item, it has turned
into a gate. Trim it. A team that cannot start work because the checklist is long is
worse off than a team with a loose checklist and a good conversation.

## Definition of Done (per increment)

The team's shared bar for "finished". Adapt, do not delete:

- [ ] Acceptance criteria met and demonstrated to the Product Owner
- [ ] Code reviewed and merged to trunk
- [ ] Automated tests added or updated; pipeline green
- [ ] Deployed to staging and smoke-tested
- [ ] No new critical or high static-analysis / security findings
- [ ] Documentation or runbook updated where behaviour changed
- [ ] Observability in place: logs, metric or alert for the new path
- [ ] Feature flag documented, with an owner and a removal date
- [ ] Release notes line written in user language

## Adding AI-assisted work to DoD

Teams using AI in delivery need three extra lines, otherwise quality quietly drifts:

- [ ] **Source disclosure** — AI-assisted artifacts (code, copy, test cases) are
  labelled where the team agreed to label them
- [ ] **No secrets, customer data or PII in prompts** — checked against the approved
  tool list
- [ ] **Human ownership** — the reviewer named on the PR or artifact is accountable
  for correctness; "the model wrote it" is not a defence

Keep estimates, performance judgements about people, and conflict decisions human.
Drafting, summarising, clustering and test scaffolding are the safe uses.

## Team working agreements for AI (starter)

1. One named workflow to start — e.g. drafting acceptance criteria — not ten at once.
2. Measure the effect on cycle time or escaped defects after four sprints.
3. Any tool that receives company data goes through security first.
4. Review the agreement every quarter; the tooling changes faster than the policy.

## Where these live

In Confluence, linked from the Jira board header, versioned, with a named owner.
A DoD nobody can find is a DoD nobody uses.
