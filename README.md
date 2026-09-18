# Neo Reception Workflow Demo

Synthetic reception workflow showing classification, availability, scarce-resource handling and escalation.

## Public scope

Local simulation only. No telephone provider, customer account or real call is connected.

## Workflow

```text
Incoming request -> classify -> check availability and constraints -> assign or escalate -> human fallback
```

The simulation makes scarce resources and escalation visible instead of hiding them inside an automated decision.

## Technical evidence contract

The internal workflow passed its tested gate, while the live voice channel remains a separate deployment decision. This repository demonstrates the decision engine with synthetic requests and no telephony provider.

Reviewers can inspect availability, shifts, scarce-resource conflicts, repeated requests and escalation. The demo proves the workflow behaviour, not live call volume or customer results.

Architecture source: `architecture.mmd`.

## Review points

- Availability and shift constraints.
- Scarce-resource conflict.
- Escalation when the workflow cannot decide safely.
- No live voice integration or customer-result claim.

## Related case study

See `../case-studies/03-neo-reception-agent.md` in the portfolio source.

## Reproducible demo

Open `demo/index.html` locally. The demo uses synthetic shifts and requests to show assignment, escalation and human fallback.
