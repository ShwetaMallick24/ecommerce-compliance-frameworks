# Seller Onboarding Playbook for High-Risk Categories

## Background

When TikTok Shop began expanding into regulated product categories, there was no existing playbook. Sellers entering categories like supplements, medical devices, or health products had to navigate complex regulatory requirements — but most small and mid-size sellers don't have in-house legal teams.

The result: high drop-off during onboarding, compliance errors post-launch, and reactive takedowns that damaged seller trust.

**The solution:** A structured, step-by-step onboarding playbook that made compliance requirements clear, sequential, and achievable — without needing a lawyer to interpret them.

---

## Design Principles

1. **Plain language over legal language.** Every requirement written so a first-time seller in a regulated category can understand it without external help.
2. **Show the finish line.** Sellers can see all steps upfront, know exactly what's required, and track their own progress.
3. **Front-load clarity, not friction.** Hard requirements surface early — before sellers invest time in listings — to avoid wasted effort.
4. **Automate what can be automated.** Checks that don't require human judgment run in the background, instantly.

---

## The Onboarding Flow

### Phase 1 — Category Eligibility Check (Automated, ~5 minutes)

Before a seller can apply to list in a regulated category, the platform checks:

- Account age (minimum 90 days active)
- Dispute and return rate (must be below category threshold)
- Prior policy violations (any Tier 3 violations → manual review required)
- Business verification status (must be complete)

**Output:** Eligible / Needs Remediation / Ineligible (with reason)

Sellers who are ineligible see a specific action plan — not a generic rejection. For example: "Your return rate is 8.2%. The threshold for this category is 5%. Here's how to improve it."

---

### Phase 2 — Documentation Submission

Sellers are presented with a category-specific document checklist. Each item includes:
- What it is (in plain language)
- Why it's required
- Where to get it
- Acceptable formats

**Example checklist for supplement sellers:**

| Document | Why Required | Where to Get It |
|----------|-------------|-----------------|
| Certificate of Analysis (CoA) | Confirms product matches label claims | Your manufacturer or third-party lab |
| Lab test from accredited facility | Verifies safety and ingredient accuracy | UL, Eurofins, NSF, or equivalent |
| Supplement Facts panel | Required by FDA for all dietary supplements | Your product label / packaging files |
| Business license | Confirms legal right to sell | Your state/local government |

Documents are uploaded directly in the seller portal. The system auto-checks file type, size, and completeness.

---

### Phase 3 — Policy Acknowledgment

Sellers complete a structured policy review — not a wall of text, but a module-based walkthrough covering:

- Prohibited claims (what you cannot say about your product)
- Packaging requirements
- Ongoing compliance obligations post-launch
- What triggers a review or takedown

Each module ends with a confirmation. This creates a documented record that the seller understood the rules — important for enforcement decisions later.

---

### Phase 4 — Review and Verification

Based on the product's risk tier (see [Risk Tiering Model](./risk-tiering-model.md)):

- **Tier 1:** Automated review. Approval notification within 48 hours.
- **Tier 2:** Category specialist review. Seller notified within 5–7 business days. Lab certification verified against approved partner list.
- **Tier 3:** Multi-team review (legal, category, operations). Seller receives status updates every 3 business days. Estimated timeline communicated upfront.

All sellers receive a decision with a specific reason — approved, approved with conditions, or rejected with a clear explanation and appeal path.

---

### Phase 5 — Launch and Ongoing Monitoring

Approved sellers go live. Post-launch monitoring is automated:

- Listing content scanned weekly for prohibited claims
- Customer complaint signals trigger review flags
- Return rate and dispute rate monitored against category thresholds
- Annual re-verification required for Tier 2 and Tier 3 sellers

Sellers receive a monthly compliance health summary in their seller dashboard.

---

## Results

- Listing-to-live time reduced by **30%** compared to the prior unstructured process
- Compliance-related takedowns reduced by **more than a third** — because sellers understood requirements before launching, not after
- Seller support tickets related to onboarding confusion dropped significantly after plain-language guides were introduced
- Smaller sellers, who previously couldn't afford legal help to navigate requirements, were able to enter regulated categories competitively

---

## TPM Lens

This playbook is fundamentally a **product spec for a workflow** — it defines the states a seller moves through, the inputs and outputs at each stage, the automated vs. manual decision points, and the edge cases (ineligible sellers, missing documents, appeal paths).

Writing it required deeply understanding both the regulatory requirements (working with legal) and the seller experience (working with operations and UX). The PM's job was to hold both simultaneously — and translate between them.

---

*Part of the [E-Commerce Compliance Frameworks](../README.md) portfolio.*
