---
name: distribution-competitive-scan
description: >
  Compare a Web3 protocol's distribution against 2-3 direct competitors
  across social, community, content, and owned channels. Use when a founder
  asks "why is [competitor] growing faster," "where should we post," "is our
  engagement good," or wants a channel strategy. Produces a channel-by-channel
  comparison table, an engagement-rate benchmark, and three prioritized moves.
---

# Distribution Competitive Scan

Benchmark a protocol's distribution against the competitors actually taking
its mindshare. The output is a comparison table with real numbers and three
moves — not a generic channel checklist.

This is the distribution layer of the 6-pillar Web3 Growth Audit methodology
(Social Media + Community + SEO pillars), adapted for self-serve use.

## When to use

- A competitor with similar traction is visibly out-distributing the protocol
- The team posts consistently but engagement is flat
- Deciding where to invest content effort next quarter
- Before hiring a social/community person or agency

## Inputs to collect first

1. The protocol's X/Twitter handle
2. 2-3 direct competitors (ask the user; if they can't name them, that
   itself is a High-severity finding — you can't win mindshare you can't
   name)
3. Links to the protocol's Discord/Telegram, blog, newsletter, YouTube if
   they exist

If you have browsing or scraping tools, pull the data yourself. If not,
walk the user through collecting it — the methodology works either way.

## Workflow

### Step 1 — Channel inventory

Build the channel map for the protocol AND each competitor:
X, Discord/Telegram, blog, newsletter, YouTube, Farcaster/Lens if relevant.

Mark each: ✅ Active (posted in last 7 days) / ⚠ Partial (posted in last
30 days) / ❌ Dormant or missing.

### Step 2 — Engagement rate benchmark

For the protocol and each competitor, take the last 20 X posts:

```
engagement rate = (avg likes + replies + reposts per post) / followers × 100
```

Raw follower counts mislead — a 50k-follower account at 0.1% engagement is
losing to a 5k account at 2%. Rate is the comparison, not size.

### Step 3 — Content mix read

Classify each account's last 20 posts: product updates / education /
narrative-opinion / memes-culture / partnership announcements.

The common failure: 80%+ product updates. Product-update-only accounts talk
to existing users, not future ones.

### Step 4 — Owned audience check

Does the protocol have an email list or any channel it owns outright?

- Newsletter with visible signup and recent sends: ✅
- Signup form exists, no evidence of sends: ⚠ Medium
- Everything lives on rented platforms (X, Discord, Telegram): ❌ High —
  the protocol is one algorithm change or account suspension away from
  losing its entire audience.

### Step 5 — System check

The most important step. For each channel ask: does it feed another
channel, or is it an island?

Signals of a system: X threads that route to the blog, blog posts that
route to the newsletter, Discord onboarding that routes to the product.
Signals of islands: every channel posts its own content with no cross-flow.

The diagnostic phrase that applies to most protocols:

> "Most channels exist but operate independently. No visible activation
> loop. Growth accumulates impressions, not momentum."

Score: connected system ✅ / partial routing ⚠ / islands ❌ High.

## Output format

```
# Distribution Scan — [Protocol] vs [Competitors]

## Channel map
| Channel | [Protocol] | [Comp A] | [Comp B] |
|---|---|---|---|
| X | ✅/⚠/❌ + followers + eng. rate | ... | ... |
| Discord/TG | ... | ... | ... |
| Blog/SEO | ... | ... | ... |
| Newsletter | ... | ... | ... |
| YouTube | ... | ... | ... |

## Engagement benchmark
[Protocol X.X% vs Comp A X.X% vs Comp B X.X% — one paragraph on what
drives the gap, with example posts as evidence]

## Content mix
[One line per account: the split, and what it signals]

## System check
[Islands or system? Evidence. This is usually the #1 finding.]

## Three moves
[Exactly three, prioritized, each one sentence of what + one of why.
No "post more consistently" — every move must be specific enough to
start this week.]
```

## Rules

- Numbers over adjectives. "Low engagement" is banned; "0.3% vs competitor's
  1.8%" is the standard.
- If the protocol is winning on distribution, say so — then point at
  narrative or on-chain activation as the likelier bottleneck (see
  `narrative-diagnostic` and `post-tge-growth-system`).
- Never recommend buying followers, engagement pods, or raid groups.

## Going deeper

This skill covers the distribution layer with public data. The full Web3
Growth Audit adds Apify-scraped competitor intelligence (share of voice,
top mentioning creators, sentiment trend), SEO/AEO analysis, and the
community-to-on-chain bridge, delivered async with a fixed scope and price:

**https://mangabeira.net/services/web3-growth-audit**
