# Sprint Planning — 120-minute agenda

For a two-week sprint, team of 5–9, one Product Owner, one Scrum Master.

## Before the meeting (Scrum Master, 15 min)

- [ ] Backlog refined: top 2 sprints' worth of stories meet DoR (`definition-of-ready-done.md`)
- [ ] Capacity sheet filled from known absence, holidays and part-time allocation
- [ ] Last sprint's carry-over and unfinished work visible on the board
- [ ] Sprint Goal candidates drafted with the Product Owner — **two options, not one**
- [ ] Room/board open, timer visible, remote link tested

## Agenda

| Time | Segment | Output |
|---|---|---|
| 0:00–0:05 | Why this sprint: Product Goal, current metrics, business context | Shared context |
| 0:05–0:15 | Capacity and constraints | Realistic number of story points / items |
| 0:15–0:30 | Sprint Goal: agree the outcome sentence | **One** Sprint Goal |
| 0:30–1:15 | Pull stories against the Goal; slice anything too big | Sprint Backlog |
| 1:15–1:30 | Task breakdown for the first 3–4 days only | First-slice tasks |
| 1:30–1:50 | Risks, dependencies, assumptions; confirm DoD per item | Risk list |
| 1:50–2:00 | Commitment check: "can we deliver the Goal?" — thumbs | Forecast |

## Capacity maths

```
Available person-days = Σ (working days in sprint − leave − ceremonies)
                        × allocation %
Focus factor          = 0.7 (use 0.6 for teams new to each other)
Sprint capacity       ≈ person-days × focus factor
```

Do not convert capacity into points by dividing last sprint's velocity. Use the
conversation to decide how much of the backlog is safe, and forecast with a range
("6–8 items"), not a single number.

## Writing the Sprint Goal

Bad: *"Complete JIRA-114 to JIRA-131."*
Good: *"Checkout is recoverable after a payment failure, so support stops handling
refund tickets manually."*

Test: could a stakeholder repeat it after reading it once, and does it explain a
user or business outcome?

## Anti-patterns to name out loud

- **Stakeholder drive-by**: someone adds a "must-have" mid-session. Park it in the
  backlog, restate capacity, offer a trade-off. Never inflate commitment silently.
- **Slicing theatre**: an item is too big but gets pulled anyway. If it cannot be
  finished in the sprint, split it now (`story-splitting.md`).
- **Task theatre**: breaking every story into 3-hour tasks for all 10 days. Break
  down the first few days only; the rest emerges.
- **Velocity as a promise**: leadership asks for "just 10% more". Answer with flow
  metrics and predictability, not with a bigger number.

## Done-when

- Sprint Goal is written on the board and readable by everyone
- Every pulled item meets DoR and has an owner
- Risks and dependencies have someone watching each
- The team forecast is a range, and the Scrum Master has written down the
  assumptions behind it
