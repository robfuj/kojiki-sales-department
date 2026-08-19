# 04 — Sales

> Part of the **Hermes Organizational Decision System**. This repo is the
> **Sales** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/hermes-ios/00-kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> How do we convert demand into revenue?

## Purpose
Convert qualified opportunities into revenue through evidence-based deal progression.

## Sub-functions
Prospecting, Account Research, Qualification, Opportunity Management, Enterprise Sales, Account Management, Solutions Engineering, Sales Operations, Deal Desk, Sales Enablement

## Typical roles
CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer

## Inputs
Leads, account intelligence, buyer signals, product information, pricing, competitive data.

## Outputs
Qualified pipeline, proposals, contracts, revenue, win/loss data.

## Learning focus
Buying signals; decision-maker patterns; blockers; win/loss patterns; qualification accuracy; next-best-action effectiveness.

## Operating tree
```text
MARKET INTELLIGENCE →
    TARGET ACCOUNT →
    STAKEHOLDER MAPPING →
    ENGAGEMENT →
    QUALIFICATION →
    ACTIVE DEAL →
    DEAL INTELLIGENCE →
    DIAGNOSIS →
    DEAL THESIS →
    STRATEGY →
    NEXT BEST ACTION →
    CUSTOMER RESPONSE →
    STATE UPDATE →
    WON / LOST / STALLED →
    POST-DEAL LEARNING
```

## Decision states
```text
PROSPECT → QUALIFIED → DISCOVERY → PROPOSAL → NEGOTIATION → WON → LOST → STALLED → NURTURE
```

## Decision outputs
`Advance · Change Strategy · Escalate · Nurture · Disqualify · Close`

## Critical prompts (what this function thinks about)
> Why will they buy?
> Why won't they buy?
> Why now?
> Why us?
> Who actually decides?
> Who influences the decision?
> Who can kill the deal?
> What is the customer's decision process?
> What evidence proves the deal is real?
> What is preventing progression?
> What assumption are we making?
> What evidence would disprove our thesis?
> What is the highest-value next action?
> What response do we expect?
> What does a negative response mean?
> Should the strategy change?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/04-sales.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
