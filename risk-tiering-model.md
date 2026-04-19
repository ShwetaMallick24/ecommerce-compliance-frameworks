# Risk Tiering Model for Regulated Marketplace Categories

## Problem Statement

Adding new regulated product categories (medical devices, supplements, cosmetics, food) to a marketplace is typically slow — most platforms launch only a handful per year. The bottleneck isn't regulatory complexity alone; it's the **absence of a structured risk framework** that lets teams move quickly on lower-risk items while applying rigorous checks where they're truly needed.

Without risk tiering, every new product gets treated the same — either everything is slow (safe but growth-limiting) or everything moves fast (growth-enabling but dangerous).

---

## The Framework

### Three-Tier Classification System

Products entering a new regulated category are classified into one of three tiers based on a scoring matrix across four dimensions.

---

#### Tier 1 — Standard Risk
**Go-live timeline: 24–48 hours**

Characteristics:
- No prescription or license required
- Established product type with clear regulatory precedent
- Low consumer harm potential if misused
- Seller has clean compliance history on platform

Examples: general wellness supplements (Vitamin C, melatonin), basic cosmetics, non-medicated skincare

Verification required:
- Standard seller identity verification
- Product listing review against category policy
- Automated content check (ingredient claims, prohibited language)

---

#### Tier 2 — Elevated Risk
**Go-live timeline: 5–7 business days**

Characteristics:
- Regulated ingredient or health claim involved
- Moderate consumer harm potential
- Category has documented history of violations platform-wide
- First time seller is listing in this category

Examples: protein powders with performance claims, topical treatments, children's health products

Verification required:
- All Tier 1 checks
- Third-party lab certification (partnered labs: UL, Eurofins)
- Manual policy review by category specialist
- Trust badge eligibility assessment

---

#### Tier 3 — High Risk
**Go-live timeline: 10–15 business days (parallel review tracks)**

Characteristics:
- Prescription-adjacent or medical device classification
- FDA/FTC oversight in the product category
- High consumer harm potential if product is misrepresented
- New or novel product type without established precedent

Examples: medical devices (blood pressure monitors, glucose meters), non-prescription health products with drug claims, weight loss supplements

Verification required:
- All Tier 1 and Tier 2 checks
- Legal team review
- Regulatory documentation (FDA registration, 510(k) clearance where applicable)
- Enhanced ongoing monitoring post-launch

---

## Scoring Matrix

Each product receives a score (1–3) across four dimensions. Average score determines tier placement.

| Dimension | Score 1 | Score 2 | Score 3 |
|-----------|---------|---------|---------|
| **Regulatory exposure** | No specific regulation | State/industry regulation | Federal regulation (FDA, FTC) |
| **Harm potential** | Low (cosmetic, general wellness) | Moderate (health claims) | High (medical, drug-adjacent) |
| **Seller history** | Clean, established | New to category | Prior violations |
| **Category precedent** | Well-established on platform | Partially established | Net new category |

**Average 1.0–1.5 → Tier 1 | 1.6–2.2 → Tier 2 | 2.3–3.0 → Tier 3**

---

## Why This Worked

**Speed without sacrificing safety.** By decoupling risk levels, Tier 1 products could go live in under 48 hours — dramatically faster than the industry average — while Tier 3 products got the scrutiny they required. This let TikTok Shop launch 12+ regulated categories in 18 months.

**Parallel review tracks.** For Tier 3 products, legal review and lab certification ran simultaneously rather than sequentially. This cut review time by ~40% without reducing rigor.

**Reduced erroneous takedowns.** Clear upfront criteria meant fewer products were removed after going live due to policy mismatches. Compliance-related takedowns dropped by more than a third.

**Seller trust.** Sellers knew exactly what they needed to provide and why. Ambiguity was replaced with a clear checklist — reducing seller frustration and platform support load.

---

## TPM Takeaway

This framework is a product decision as much as a compliance one. The risk tiers are essentially a **product spec for the onboarding flow** — they define what the system needs to check, in what order, and how to route each product through the right review pipeline.

Building it required alignment across engineering (automated checks), legal (regulatory standards), operations (review capacity), and seller experience (documentation requirements). Getting all of those to agree on a single framework is the core PM challenge.

---

*Part of the [E-Commerce Compliance Frameworks](../README.md) portfolio.*
