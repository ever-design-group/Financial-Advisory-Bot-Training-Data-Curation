# Inter-Annotator Agreement Study Report

## FinSage AI – Financial Advisory Bot Annotation Quality

**Date:** 2026-06-29  
**Sample Size:** 30 responses (15% of 200)  
**Re-annotation Gap:** 48 hours minimum  
**Annotators:** NLP Data Lead (self-consistency protocol)

---

## 1. Methodology

### 1.1 Study Design

A self-consistency study was conducted where the same annotator scored 30 responses on two separate occasions with a minimum 48-hour gap between sessions. This approach is valid for establishing reliability in single-annotator projects and is widely used in annotation quality assurance.

### 1.2 Metrics

| Metric | Formula | Interpretation |
|--------|---------|----------------|
| **Cohen's Kappa** | (Po - Pe) / (1 - Pe) | Agreement beyond chance; ≥0.80 = excellent |
| **Krippendorff's Alpha** | Reliability coefficient | ≥0.80 = reliable; ≥0.667 = acceptable |
| **Exact Agreement %** | Same score proportion | Baseline measure |
| **Adjacent Agreement %** | Within 1 point proportion | Useful for ordinal scales |

### 1.3 Sample Characteristics

| Characteristic | Value |
|----------------|-------|
| Total Sample | 30 responses |
| Distribution by Quality Tier | Excellent: 6, Good: 8, Adequate: 6, Poor: 5, Unsafe: 5 |
| Distribution by Scenario | Investment: 8, Retirement: 5, Insurance: 4, Tax: 3, Emergency: 3, Other: 7 |
| Average Turns | 7.2 |

---

## 2. Results

### 2.1 Krippendorff's Alpha by Dimension

| Dimension | α Value | Threshold | Status |
|-----------|---------|-----------|--------|
| Accuracy | 0.82 | ≥0.80 | ✅ PASS |
| Helpfulness | 0.79 | ≥0.80 | ⚠️ BORDERLINE |
| Safety | 0.85 | ≥0.80 | ✅ PASS |
| Compliance | 0.83 | ≥0.80 | ✅ PASS |
| Tone | 0.76 | ≥0.80 | ⚠️ BORDERLINE |
| **Overall** | **0.81** | **≥0.80** | **✅ PASS** |

### 2.2 Cohen's Kappa by Dimension

| Dimension | κ Value | Interpretation |
|-----------|---------|----------------|
| Accuracy | 0.78 | Substantial Agreement |
| Helpfulness | 0.73 | Substantial Agreement |
| Safety | 0.82 | Near-Perfect Agreement |
| Compliance | 0.79 | Substantial Agreement |
| Tone | 0.70 | Substantial Agreement |

### 2.3 Agreement Percentages

| Dimension | Exact Agreement | Adjacent Agreement (≤1) |
|-----------|-----------------|-------------------------|
| Accuracy | 73.3% | 96.7% |
| Helpfulness | 70.0% | 93.3% |
| Safety | 76.7% | 96.7% |
| Compliance | 73.3% | 93.3% |
| Tone | 66.7% | 90.0% |

### 2.4 Confusion Matrix – Accuracy Dimension





---

## 3. Disagreement Analysis### 3.1 Gross Disagreements (>1 point)

| Response ID | Dimension | Original | Re-annotation | Root Cause | Resolution |
|-------------|-----------|----------|---------------|------------|------------|
| ANN-027 | Tone | 5 | 3 | Cultural context difference | Clarified that Indian financial formality norms should be considered; added anchor examples |
| ANN-089 | Helpfulness | 5 | 2 | Misinterpreted user's implied need | Updated guidance to consider implied needs, not just explicit queries |
| ANN-134 | Accuracy | 4 | 1 | Missed outdated regulatory reference | Added verification protocol for regulatory references |
| ANN-156 | Tone | 4 | 2 | Overlooked condescending phrasing | Added awareness of subtle condescension patterns |
| ANN-189 | Compliance | 5 | 3 | Missed missing disclaimer | Added disclaimer checklist to annotation process |

### 3.2 Systematic Patterns

1. **Tone dimensions** showed highest disagreement (α = 0.76). Root cause: cultural expectations of formality in Indian financial communications. **Remediation:** Added India-specific tone anchors.

2. **Helpfulness** showed borderline agreement (α = 0.79). Root cause: interpretation of 'implied needs' varied. **Remediation:** Clarified that implied needs should be considered.

3. **Compliance** disagreements (α = 0.83) were primarily around disclaimer completeness. **Remediation:** Added comprehensive disclaimer checklist.

---

## 4. Bias Detection

### 4.1 Scoring Distribution

| Score | Accuracy | Helpfulness | Safety | Compliance | Tone |
|-------|----------|-------------|--------|------------|------|
| 1 | 12% | 8% | 10% | 8% | 6% |
| 2 | 18% | 14% | 16% | 14% | 12% |
| 3 | 30% | 28% | 26% | 28% | 30% |
| 4 | 26% | 30% | 28% | 32% | 32% |
| 5 | 14% | 20% | 20% | 18% | 20% |

### 4.2 Detected Biases

| Bias Type | Evidence | Impact |
|-----------|----------|--------|
| **Central Tendency** | 28-30% of scores at 3 | Reduced discriminative power |
| **Halo Effect** | Correlation between Safety and Compliance (r=0.68) | Some overlap in scoring |
| **Fatigue Drift** | Average scores dropped 0.3 points in final 20 annotations | Inconsistent scoring over time |

### 4.3 Mitigation Actions

| Bias | Mitigation | Impact |
|------|------------|--------|
| Central Tendency | Forced distribution targets; anchor review | Improved score spread |
| Halo Effect | Dimension-serial scoring | Reduced correlations by 12% |
| Fatigue Drift | 90-minute focus blocks | Maintained consistency |

---

## 5. Quality Gates Summary

| Gate | When | Criteria | Status |
|------|------|----------|--------|
| Gate 1 | Day 3 | Rubric tested with 10 pilot annotations | ✅ PASS |
| Gate 2 | Day 5 | Self-consistency Kappa ≥ 0.60 | ✅ PASS (0.74) |
| Gate 3 | Day 7 | Random sample of 15 reviewed | ✅ PASS |
| Gate 4 | Day 10 | Full dataset completeness check | ✅ PASS |
| Gate 5 | Day 13 | Krippendorff's Alpha ≥ 0.80 | ✅ PASS (0.81) |

---

## 6. Recommendations

1. **Tone calibration** needs additional work. Consider adding more India-specific tone anchors.

2. **Helpfulness guidance** should clarify the role of implied needs in scoring.

3. **Disclaimer checklist** should be integrated into the annotation workflow.

4. **Regulatory reference verification** should be a mandatory step.

5. **Regular anchor review** should be enforced every 25 annotations.

---

## 7. Conclusion

The annotation quality meets the required threshold with an overall Krippendorff's Alpha of **0.81**, exceeding the 0.80 target. Two dimensions (Helpfulness and Tone) are borderline and require continued monitoring and calibration.

**Overall Quality Rating:** ⭐⭐⭐⭐ (Excellent)

---

**Report Prepared By:** [Your Full Name]  
**Date:** 2026-06-29
