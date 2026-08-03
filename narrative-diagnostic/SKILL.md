---
name: narrative-diagnostic
description: >
  Diagnose a Web3 protocol's narrative across its website and social surfaces.
  Use when a founder or marketer asks "is our messaging working," "why isn't
  our story landing," "audit our positioning," or wants to know why traffic
  doesn't convert. Works for DeFi, DePIN, stablecoins, wallets, RWA, and
  infrastructure protocols. Produces a scored narrative scorecard with
  severity flags and concrete rewrites, never generic advice.
---

# Narrative Diagnostic

Run a structured narrative audit on a Web3 protocol. The output is a scorecard
with evidence, severity flags, and rewrites — not opinions.

This is the narrative layer of the 6-pillar Web3 Growth Audit methodology
(Website + Social Media pillars), adapted for self-serve use.

## When to use

- The protocol has traffic or followers but weak conversion
- The team can't explain what they do in one sentence without jargon
- A competitor with a worse product is out-narrating them
- Before spending on ads, KOLs, or a rebrand

## Inputs to collect first

Ask the user for (or fetch if you have browsing tools):

1. Homepage URL
2. Docs or litepaper URL
3. X/Twitter handle (bio + pinned post + 10 most recent posts)
4. The team's own one-sentence description of the protocol
5. Who they believe their ideal user is

Do not start scoring until you have at least the homepage and the X bio.
Missing surfaces are findings, not blockers — mark them ❌ MISSING.

## Workflow

### Step 1 — The one-sentence test

Read only the homepage hero (headline + subline). Write down, without
scrolling further: what does this protocol do, for whom, and why should
that person care?

- If you can answer all three: ✅
- If you can answer one or two: ⚠
- If you're guessing or the answer is category jargon ("the liquidity layer
  for modular restaking"): ❌ Critical

### Step 2 — ICP clarity

From the homepage and docs, identify who this is written for. Score:

- Named, specific user with a named problem: ✅
- "Traders / users / everyone in DeFi": ⚠ High
- Written for other builders or VCs instead of users: ❌ Critical

### Step 3 — Differentiation

List the protocol's claimed differentiators. For each one, ask: could a
direct competitor paste this claim onto their own site unchanged?

- At least one claim only this protocol can make: ✅
- All claims are category table stakes (fast, secure, decentralized,
  audited): ❌ High

### Step 4 — Proof and evidence

Inventory every number, integration logo, audit badge, and user quote on
the homepage. Score:

- Specific, verifiable numbers (TVL, users, transactions) with sources: ✅
- Vague social proof ("trusted by thousands") or none: ❌ High
- Numbers that contradict public data (check DefiLlama/CoinGecko if
  available): ❌ Critical — flag explicitly, this destroys trust

### Step 5 — Message consistency

Compare: homepage headline vs X bio vs pinned post vs docs intro.
They should tell one story at different depths.

- Same positioning, same vocabulary: ✅
- Different framings per surface (site says "payments," X bio says
  "RWA infra"): ❌ High — this is the most common Web3 narrative failure

### Step 6 — Jargon test

Take the hero copy and X bio. Count terms that require Web3-insider
knowledge beyond the protocol's actual ICP. A DeFi power-user ICP tolerates
"restaking." A mainstream wallet ICP does not.

- Jargon matches ICP sophistication: ✅
- Jargon exceeds ICP sophistication: ⚠ Medium (High if ICP is mainstream)

## Output format

Produce exactly this structure:

```
# Narrative Diagnostic — [Protocol]

## Scorecard
| Check | Status | Severity | Evidence |
|---|---|---|---|
| One-sentence test | ✅/⚠/❌ | — /Medium/High/Critical | [quote the actual copy] |
| ICP clarity | ... | ... | ... |
| Differentiation | ... | ... | ... |
| Proof & evidence | ... | ... | ... |
| Message consistency | ... | ... | ... |
| Jargon test | ... | ... | ... |

## The #1 narrative gap
[One paragraph. The single finding that, fixed first, unlocks the most.
Quote the current copy as evidence.]

## Rewrites
[For each ❌ finding: current copy → suggested copy. Match the protocol's
existing tone. No hype vocabulary: never "revolutionary," "game-changing,"
"unlock," "seamless."]

## What this diagnostic can't see
[1-3 lines. Be honest: conversion data, on-chain funnel, community health,
and competitive share of voice are outside this skill's scope.]
```

## Rules

- Every claim needs quoted evidence from the actual surface. No abstract
  criticism.
- Severity is about business impact, not aesthetics.
- If every check passes, say so plainly and point to distribution or
  on-chain activation as the more likely bottleneck (see the companion
  skills `distribution-competitive-scan` and `post-tge-growth-system`).

## Going deeper

This skill covers the narrative layer. The full Web3 Growth Audit runs all
six pillars — Website, dApp, Social, Community, SEO, PR — with on-chain
cohort data (Dune) and competitive social intelligence, delivered async
with a fixed scope and price:

**https://mangabeira.net/services/web3-growth-audit**
