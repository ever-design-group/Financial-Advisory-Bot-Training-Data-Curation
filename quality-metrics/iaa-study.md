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
