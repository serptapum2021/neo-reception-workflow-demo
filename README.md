# Neo Reception Workflow Demo

Synthetic reception workflow showing classification, availability, scarce-resource handling and escalation.

## Public scope

Local simulation only. No telephone provider, customer account or real call is connected.

## Workflow

```text
Incoming request -> classify -> check availability and constraints -> assign or escalate -> human fallback
```

The simulation makes scarce resources and escalation visible instead of hiding them inside an automated decision.

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
