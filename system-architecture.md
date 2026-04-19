# System Architecture: TikTok Shop Compliance Infrastructure

This diagram shows how the compliance system components connect — from seller entry through risk tiering, review tracks, trust badging, and ongoing monitoring.

## How to read this

- **Gray boxes** — entry points and rejection/remediation paths
- **Purple boxes** — platform systems (automated logic, algorithms)
- **Teal boxes** — approved/success paths
- **Amber/Coral boxes** — Tier 2 and Tier 3 review tracks (elevated and high risk)

## The flow

```
Seller Portal
      ↓
Eligibility Check (automated)
      ↓
Risk Scoring Engine → 4-dimension matrix assigns Tier 1, 2, or 3
      ↓
┌─────────────┬──────────────┬──────────────┐
│   Tier 1    │   Tier 2     │   Tier 3     │
│ Automated   │ Specialist   │ Legal + ops  │
│ 48 hrs      │ Lab cert     │ Parallel     │
└─────────────┴──────────────┴──────────────┘
      ↓ (all tiers converge)
Listing Approved + Policy Acknowledgment Logged
      ↓
┌────────────────────┬──────────────────────┐
│  Trust Badge       │  Search Ranking      │
│  Lab cert → badge  │  Compliance score    │
│  5–7% conv. lift   │  feeds visibility    │
└────────────────────┴──────────────────────┘
      ↓
Ongoing Monitoring
(weekly scans, return rate tracking, annual re-verification)
```

## Key design decisions

**Why risk tiering?**
Without tiering, every product moves at the speed of the slowest review. Separating Tier 1 (48-hour automated) from Tier 3 (multi-team review) allowed the platform to launch 12+ categories in 18 months — 3x the industry average — while maintaining safety standards for high-risk products.

**Why parallel review tracks for Tier 3?**
Legal review and lab certification previously ran sequentially. Running them simultaneously cut Tier 3 review time by ~40% without reducing rigor.

**Why connect compliance to search ranking?**
Tying visibility to compliance status created a direct economic incentive for sellers. Compliant sellers discovered that investing in verification improved their discoverability — closing the loop between compliance and revenue.

**Why log policy acknowledgment?**
Creating a documented record that sellers understood the rules before listing transformed enforcement from reactive (takedown after violation) to proactive (sellers take ownership of compliance). This was a key driver of the 33% reduction in compliance-related takedowns.

## Systems involved

| System | Function | Who built it |
|--------|----------|-------------|
| Eligibility check engine | Automated gating based on account history | Engineering |
| Risk scoring matrix | 4-dimension classification logic | PM-designed, engineering-built |
| Document verification pipeline | CoA ingestion + lab partner validation | Engineering |
| Trust badge renderer | Badge display across listing surfaces | Engineering |
| Compliance-to-ranking signal | Feeds compliance score to search algorithm | Engineering (search team) |
| Monitoring dashboard | Weekly automated scans + seller health summary | Engineering + Operations |

## What I owned as PM

I did not write the code for these systems. My role was to:

- Define the logic: what qualifies a seller for each tier, what triggers a takedown, what earns a badge
- Write the PRDs and specs that engineering built from
- Align 50+ stakeholders across engineering, legal, operations, and policy on a single framework
- Measure outcomes and iterate on the design based on data

This is the core TPM skill: designing the system's behavior, not implementing it.

---

*Part of the [E-Commerce Compliance Frameworks](./README.md) portfolio.*
