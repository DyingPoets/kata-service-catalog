# Service Catalog — Success Metrics + Acceptance Tests

> **Branch:** `skill/metrics-tests`
> **Skills:** S1 · T5 · M1
> **Audience:** PM · Eng

---

## For the Facilitator

### Session Overview

| | |
|---|---|
| **Kata** | 8: Service Catalog |
| **Session** | Success Metrics + Acceptance Tests |
| **Skills** | S1 · T5 · M1 |
| **Duration** | 2 hours (facilitated) + self-directed extension |
| **Slide Deck** | https://gamma.app/docs/703r0vlgubk3llq |
| **Miro Board** | https://miro.com/app/board/uXjVG8Q3ixk%3D/ |

### Session Timing

| Time | Activity |
|------|----------|
| 0:00–0:15 | Concept framing — open the Gamma slide deck and walk through each slide |
| 0:15–0:30 | Orient to Miro board + this starting state |
| 0:30–1:05 | Step 1 exercise (Miro — Context frame) |
| 1:05–1:25 | Step 2 exercise (Miro — Exercise frame) |
| 1:25–1:30 | Step 3 wrap-up |
| 1:30–1:50 | Debrief — use Miro Debrief frame prompts |
| 1:50–2:00 | Extension brief — point to Extension Zone in Miro |

### What to Watch For

- Metrics that can't be instrumented — "customer satisfaction" without a mechanism is not a metric
- Acceptance tests that test UI rather than behaviour — the same principles as BDD kata apply
- Analytics events without properties — "button clicked" is useless without context

### Facilitation Tips

- For each metric: "What query would you run to compute this?" — if they can't answer, the metric isn't defined
- For analytics events: "What properties do you need to answer your top 3 questions about this event?"
- Pair PM (writes metric intent) + Eng (writes instrumentation plan) for maximum depth

### Extension / Coaching Office Hours

Participants can continue extension work independently and bring it to **Coaching Office Hours**.
At Office Hours, focus on: what decision did they make, why, and what would they change?

---

## For Participants (Developer · PM · UX)

### Getting Started

```bash
git clone https://github.com/DyingPoets/kata-service-catalog
git checkout skill/metrics-tests
```

Open the Miro board and the Gamma slide deck — have both visible during the session.

- **Slides:** https://gamma.app/docs/703r0vlgubk3llq
- **Miro Board:** https://miro.com/app/board/uXjVG8Q3ixk%3D/

### What You'll Practice

- S1
- T5
- M1

### Your Starting State

You have:
- `approved-wireframes/catalog-screens.md` — approved screens from Session 1
- `templates/metrics-template.md` — template for defining metrics

Your goal: define 3 metrics, write BDD acceptance tests, and produce an instrumentation plan for metric 1.

### Step by Step

**Step 1:** Define 3 metrics. For each: what user behaviour it measures, how to instrument it, what "good" looks like at 30 days.

**Step 2:** Write acceptance tests for the catalog homepage and request flow in BDD format.

**Step 3:** Produce the instrumentation plan for metric 1: events, properties, query to compute the metric.

### What Good Looks Like

Metrics with a clear computation query. Acceptance tests that read as business rules. An instrumentation plan detailed enough for an engineer to implement without a meeting.

See the `solutions/` directory for reference examples — but try the exercise first.

### Extension Work

- Design the full analytics instrumentation for all 3 metrics
- Mock the 30-day dashboard: what 3 numbers would you show stakeholders on day 30?
- Write the acceptance tests for the IT admin view (service management side)

Bring your extension work to **Coaching Office Hours**. You'll get 15 minutes of focused feedback.

---

Part of the [PDLC Training Katas](https://github.com/DyingPoets) series.
