---
name: post-tge-growth-system
description: >
  Audit a Web3 protocol's growth system in the first months after token
  launch. Use when a founder says "we launched and growth stalled," "TVL is
  bleeding," "holders are leaving," or asks what to fix first post-TGE.
  Separates real growth failure from market beta, maps where the funnel
  leaks, and produces a prioritized 90-day fix list.
---

# Post-TGE Growth System

Diagnose why growth stalled after token launch, and what to fix first.
The output is a leak map with severity flags and a 90-day priority list —
not a pep talk and not a list of 40 tactics.

This is the on-chain and systems layer of the 6-pillar Web3 Growth Audit
methodology (dApp + Community pillars plus the attribution stack),
adapted for self-serve use.

## When to use

- Token launched in the last ~6 months and price/TVL/holders are declining
- Wallet connects happen but transactions don't follow
- The team can't tell which marketing spend produced which on-chain result
- Deciding what to fix first with a small team and limited runway

## Inputs to collect first

1. Token ticker + chain, launch date
2. Where the numbers live: DefiLlama/Dune/CoinGecko links if they have them
3. The core on-chain action a user should take (stake, deposit, mint, trade)
4. What marketing they're currently running
5. Their attribution setup, if any (GA4, Cookie3, UTM discipline, none)

## Workflow

### Step 1 — Beta check: is this actually a growth failure?

Before diagnosing anything, separate protocol failure from market beta.
Web3 tokens are heavily correlated to BTC.

- Price: token return over the window minus BTC return over the same window
- TVL: protocol TVL trend minus sector-wide TVL trend (DefiLlama)

A token down 40% while BTC is down 35% is market movement, not a marketing
failure — and "fixing marketing" won't fix it. A token meaningfully
underperforming its benchmark has a real narrative or distribution problem.

State the verdict explicitly before continuing. If the protocol merely
tracked the market down, say so — that finding alone prevents a quarter of
wasted panic spend.

### Step 2 — Funnel walk

Trace the actual user path: discovery → website → wallet connect → first
transaction → repeat transaction. For each step, what does the data show
(or what data is missing)?

The most common leak: connects without first transactions. The dApp has
no activation sequence — nothing guides a connected wallet to the core
action. Mark each step ✅ / ⚠ / ❌ with evidence.

### Step 3 — Activation loop inventory

List every mechanism that turns a new user into a repeat user: incentives,
streaks, notifications, email sequences, quests, community roles tied to
on-chain actions. For each: does it bridge to the core on-chain action, or
does it reward activity that never touches the chain?

- At least one loop that reliably produces repeat core actions: ✅
- Loops exist but reward off-chain activity (Discord messages, X raids): ⚠ High
- No loops — growth is 100% acquisition, 0% retention: ❌ Critical

### Step 4 — Attribution stack check

- UTM discipline: are campaign links tagged, consistently?
- Wallet-connect capture: does the UTM survive to the connect event?
- On-chain join: can any acquisition source be tied to any transaction?

If the answer to the third is no: every budget decision is a guess. Mark
❌ Critical. This is the single most common post-TGE infrastructure gap.

### Step 5 — Owned audience check

Same check as the distribution scan, because post-TGE it becomes acute:
when incentives taper, can the protocol reach its users without paying an
algorithm? Email list ✅ / signup-only ⚠ / nothing ❌ High.

### Step 6 — Synthesis

One paragraph answering: **where does this protocol have presence without
a system?** Tie the leaks together into a single diagnosis. The pattern to
look for:

1. Channels exist, system doesn't
2. Impressions accumulate, users don't
3. The on-chain funnel leaks before it starts
4. The attribution gap collapses budget defensibility
5. Owned audience is zero

## Output format

```
# Post-TGE Growth System — [Protocol]

## Beta check
[Underperforming benchmark, or tracking the market? Numbers + verdict.]

## Leak map
| Funnel step | Status | Severity | Evidence |
|---|---|---|---|
| Discovery → site | ... | ... | ... |
| Site → connect | ... | ... | ... |
| Connect → first TX | ... | ... | ... |
| First TX → repeat | ... | ... | ... |
| Attribution | ... | ... | ... |
| Owned audience | ... | ... | ... |

## Synthesis
[The one-paragraph diagnosis: presence without a system, and where.]

## 90-day priority list
[Exactly three fixes, ordered. For each: what, why it's first/second/third,
and the observable signal that proves it worked. Fixing the biggest leak
beats optimizing any single channel.]
```

## Rules

- Never skip the beta check. Diagnosing a market-wide drawdown as a
  marketing failure is the most expensive mistake this skill exists to
  prevent.
- Every severity flag needs evidence: a number, a screenshot-able state,
  or an explicit "no data exists — which is the finding."
- Three fixes, not ten. A post-TGE team in decline has no capacity for ten.

## Going deeper

This skill runs on public data and the team's own numbers. The full Web3
Growth Audit adds Dune cohort retention curves, connect→TX funnel queries,
wallet-cohort analysis by acquisition source, and a full 90-day roadmap
with a recorded walkthrough, delivered async with a fixed scope and price:

**https://mangabeira.net/services/web3-growth-audit**
