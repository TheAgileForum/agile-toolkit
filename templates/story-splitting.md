# Story splitting — SPIDR and INVEST

A story is too big when the team cannot finish it inside one sprint, or when nobody
can demo it on its own. Split by value, not by layer.

## INVEST, quickly

Independent · Negotiable · Valuable · Estimable · Small · Testable.
If a story fails "Valuable" and "Testable", the split went wrong — you produced a
task, not a story.

## SPIDR

| Technique | Split by | Example |
|---|---|---|
| **S**pike | Research vs build | "Investigate OAuth providers" then "Add Google sign-in" |
| **P**aths | Workflow branch | "Checkout: happy path" / "Checkout: card declined" |
| **I**nterfaces | Channel or surface | "Search on web" / "Search API for mobile" |
| **D**ata | Subset of data | "Import CSV under 10k rows" / "Import 10k+ with batching" |
| **R**ules | Business rule | "Free shipping over ₹999" / "Free shipping for members" |

## Worked splits

**Too big:** "Users can manage their profile."

1. View profile (name, email, photo) — read only
2. Edit display name and photo
3. Change email with verification
4. Delete account with 30-day grace period
5. Download my data export

Each is demoable, each has a clear acceptance test, and 1–2 deliver value in the
first sprint while the rest is scheduled on evidence.

**Too big:** "Integrate payment gateway."

1. Spike: compare gateway SDKs against our refund requirement — timeboxed 2 days
2. Accept payment for one product, sandbox only
3. Persist transaction and show it in admin
4. Handle decline and timeout paths
5. Refunds and partial refunds
6. Production credentials, monitoring and alerting

The spike is legitimate work and should be scheduled as such, not smuggled into an
estimate.

## Splitting smells

- Every slice is "backend" or "frontend" only → split by path or outcome instead
- Slices cannot be demonstrated → too thin, or not vertical
- A slice has no user → question whether it is needed this PI
- The split created 9 one-point items → group them, or the board becomes noise

## Estimation after splitting

Re-estimate after the split; do not divide the original estimate by the number of
slices. Size relative to a known small story, and stop arguing past two minutes —
if the team cannot agree, the slice is not understood well enough yet.
