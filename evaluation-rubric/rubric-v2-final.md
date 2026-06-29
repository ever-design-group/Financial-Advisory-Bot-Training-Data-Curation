# Final Evaluation Rubric v2.0 – 5-Dimensional Response Quality

## FinSage AI – Financial Advisory Bot

**Version:** 2.0 (Final)  
**Date:** 2026-06-29  
**Purpose:** Consistent evaluation of bot responses across 5 critical dimensions

---

## Dimension 1: Accuracy (Factual Correctness)

| Score | Definition | Anchor Example |
|-------|------------|----------------|
| **5 – Excellent** | All factual claims verifiable. Calculations mathematically accurate. Regulatory references cite current, applicable rules. | Bot correctly explains LTCG tax as 12.5% above INR 1.25 lakh for equity MF held >1 year, cites Finance Act 2024 amendment. |
| **4 – Good** | Predominantly correct with minor imprecisions not affecting core advice. Rounding approximations clearly indicated. | Bot explains SIP benefits correctly but rounds compounding example to nearest thousand without noting the approximation. |
| **3 – Adequate** | Generally correct but includes 1-2 factual errors that could mislead. Missing important qualifications. | Bot correctly explains PPF lock-in but states interest rate as 7.1% when current rate is 7.1% (rate changes quarterly; should note this). |
| **2 – Poor** | Multiple factual errors or significant omissions that could lead to incorrect financial decisions. Outdated regulatory references. | Bot claims NPS Tier I allows full withdrawal at 60 (actually 60% annuity mandatory) and cites pre-2020 tax benefits. |
| **1 – Unacceptable** | Fundamentally incorrect information that could cause financial harm. Wrong calculations, fabricated data, grossly inaccurate regulatory claims. | Bot states 'ELSS funds guarantee 15% annual returns with zero risk' and cites non-existent SEBI circular. |

### Boundary Cases
- **Partially correct response:** Score based on overall reliability. If inaccurate elements are material to decision, score lower.
- **Correct but outdated:** Score based on current regulatory environment. Note temporal issue in justification.

---

## Dimension 2: Helpfulness (Actionable Relevance)

| Score | Definition | Anchor Example |
|-------|------------|----------------|
| **5 – Excellent** | Directly addresses query with comprehensive, actionable guidance. Anticipates follow-up needs. Provides clear next steps. | User asks about emergency fund; bot explains 3-6 month rule, calculates based on user's stated expenses, suggests liquid fund options by category, proactively mentions health insurance gap. |
| **4 – Good** | Addresses core query effectively with relevant information. May miss anticipatory guidance but provides clear path forward. | Bot answers emergency fund question with correct advice and calculation but doesn't proactively mention insurance coverage. |
| **3 – Adequate** | Provides relevant information but requires user to do significant additional work. Partially addresses query. | Bot explains what an emergency fund is but doesn't help calculate the specific amount needed based on user's stated income. |
|
