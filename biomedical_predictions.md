# Biomedical Predictions: PCP-Lattice Guided Drug Discovery

**Quantitative, falsifiable predictions for cancer, Alzheimer's, and degenerative diseases**  
**Derived from the PCP-Lattice verification framework (Moses Kelley, February 2026)**

---

## Preamble: Prediction Criteria

Every prediction below satisfies the same five criteria used for the cosmological predictions:

1. **Quantitative** — gives a number, not just a direction
2. **Falsifiable** — specific enough to be wrong
3. **Distinct** — different from standard pharmacological models
4. **Testable** — within a decade with existing clinical infrastructure
5. **Derived** — from the internal logic of PCP-Lattice, not ad hoc

---

## Tier 1: Testable Within 3 Years (2026–2028)

### Prediction B1: Kinase Inhibitor Response Time Correlation

**Statement:** For targeted kinase inhibitors in oncology, the time to initial tumour response (≥30% marker reduction) correlates with the PCP-predicted transition time:

```
t_response = τ × (1 / 0.30 − 1)^{1/β}
```

with `τ` calibrated from the drug's PK half-life and `β` from its dose-response steepness.

**Quantitative target:** The PCP formula predicts `t_response` within ±2 months of observed median for drugs with known `τ` and `β`, corresponding to r² > 0.60 across ≥10 approved kinase inhibitors.

**Test:** Retrospective analysis of FDA-approved kinase inhibitors (imatinib, erlotinib, crizotinib, osimertinib, sotorasib, etc.) using published Phase III time-to-response data.

**Discrimination from standard PK/PD:** Standard E_max models require fitting 3–4 parameters per drug. The PCP model uses 2 (`τ`, `β`) with `γ_bio` derived from binding-affinity data.

---

### Prediction B2: Anti-Amyloid Efficacy Threshold

**Statement:** Anti-amyloid therapies targeting proteins with PCP verification error `ε < 0.20` will show statistically significant amyloid reduction (>25% SUVr decrease) at 18 months, while those with `ε > 0.25` will fail to reach significance.

```
ε = ξ_drug / √(N_residues^{d_eff})
```

**Quantitative target:**
- Lecanemab (targets Aβ protofibrils, ~42–100 residue aggregates): `ε ≈ 0.21–0.26` → borderline, consistent with its modest 27% slowing
- Donanemab (targets N-truncated Aβ, ~42 residues): `ε ≈ 0.26` → predicts marginal effect
- A hypothetical antibody targeting larger tau aggregates (441 residues): `ε ≈ 0.19` → predicts stronger effect

**Test:** Compare ε values against clinical trial outcomes for all anti-amyloid/anti-tau antibodies reaching Phase III by 2028.

---

### Prediction B3: Combination Synergy Detection

**Statement:** Drug combinations with PCP-predicted synergy ratio > 1.15 will show hazard ratio improvements > 20% over the best monotherapy, detectable in Phase II trials with N ≥ 200.

```
Synergy ratio = ξ_combined / ξ_additive
ξ_combined = √(ξ₁² + ξ₂² + 2 × interaction × ξ₁ × ξ₂)
```

**Quantitative target:** For checkpoint inhibitor + chemotherapy combinations in NSCLC, the synergy ratio calculated from binding-affinity data should predict the observed hazard ratio improvement with correlation r > 0.50.

**Test:** Retrospective analysis of KEYNOTE-189, CheckMate-227, and IMpower150 combination trial data.

---

## Tier 2: Testable Within 5 Years (2026–2030)

### Prediction B4: Neuroprotective Dosing Window

**Statement:** The optimal treatment duration for neuroprotective agents follows:

```
t_optimal = τ × (1 / 0.50 − 1)^{1/β} = τ  (for β = 1)
```

Treating beyond `2 × t_optimal` provides < 10% additional benefit (diminishing returns from the relaxation profile's tail).

**Quantitative target:** Clinical trials of riluzole, edaravone, and tofersen in ALS should show that > 80% of total benefit accrues within the first `t_optimal` months.

**Test:** Time-partitioned efficacy analysis of existing ALS trial data.

---

### Prediction B5: Multi-Target Composite Score

**Statement:** Drug candidates with PCP composite score > 150 (on the standardised scale) will have Phase II success rates > 30%, compared to the industry average of ~15%.

```
Score = Efficacy × Window / (1 + 100 × ε)
```

**Quantitative target:** A prospective ranking of 20 oncology candidates using PCP composite scoring will show AUC > 0.70 for predicting Phase II success/failure.

**Test:** Apply PCP scoring to oncology drug pipelines (public data from ClinicalTrials.gov) and track outcomes.

---

### Prediction B6: Binding-Affinity Sweet Spot

**Statement:** The therapeutic index (efficacy / toxicity) is maximised when the binding-affinity parameter falls in the range:

```
0.20 < γ_bio < 0.35
```

corresponding to `ξ_drug` between 0.34 and 0.62.

Outside this range:
- `γ_bio < 0.15` → ξ_drug < 0.25 → insufficient efficacy (< 5%)
- `γ_bio > 0.45` → ξ_drug > 0.85 → excessive on-target toxicity

**Quantitative target:** > 70% of FDA-approved small-molecule drugs in oncology and neurology fall within `0.15 < γ_bio < 0.40` when γ_bio is estimated from IC50 and selectivity data.

**Test:** Map IC50 values of approved drugs to γ_bio using the binding-affinity calibration and verify the distribution.

---

## Tier 3: Testable Within 10 Years (2026–2035)

### Prediction B7: Protein-Lattice Verification as a Drug Design Objective

**Statement:** Using `ε < 0.10` as a design constraint in computational drug discovery will produce lead compounds with > 2× higher clinical success rates than unconstrained design.

```
ε = ξ_drug / √(N_target^{d_eff})
```

To achieve `ε < 0.10`, either:
- Target large proteins (N > 700 residues), or
- Use drugs with lower γ_bio (< 0.15, but sacrifice efficacy), or
- Design multi-valent drugs that increase effective N

**Test:** Prospective trial in AI-guided drug discovery platforms (e.g., Recursion, Insilico Medicine, Isomorphic Labs).

---

### Prediction B8: Disease Progression Universality

**Statement:** The PCP disease-progression equation:

```
P(t) = P_baseline × [1 + (ξ_pathology / 2) × (1 − f(t)) × s_max]
```

with appropriate `γ_pathology`, `τ`, and `β` fits disease-progression curves for cancer, Alzheimer's, Parkinson's, and ALS with residuals < 10% RMS — demonstrating **universality** across disease categories.

**Quantitative target:** The 3-parameter PCP model (`γ`, `τ`, `β`) fits as well as or better than disease-specific 4–6 parameter models currently used in clinical trial design.

**Test:** Fit PCP progression curves to natural-history datasets from ADNI (Alzheimer's), PRO-ACT (ALS), PPMI (Parkinson's), and SEER (cancer).

---

### Prediction B9: The Biomedical Hubble Constant

**Statement:** Just as H₀ = 73.01 km/s/Mpc emerges from the PCP framework as a universal expansion rate, a "biomedical Hubble constant" emerges as the universal maximal efficacy:

```
E_max_universal = (ξ_default / 2) × s_max × 100 = 8.39%
```

This predicts that **no single-agent monotherapy** can reduce a disease biomarker by more than ~8–9% through binding-affinity mechanisms alone. Larger effects require:
- Combination therapy (dual-lattice enhancement)
- Mechanism-of-action beyond binding (e.g., degraders, gene therapy)
- Modifying the biological γ_bio through drug design

**Test:** Survey Phase III efficacy data across therapeutic areas and verify the ~8–9% ceiling for single-mechanism drugs.

---

## Tier 4: Foundational Predictions (2035+)

### Prediction B10: PCP-Guided Personalised Medicine

**Statement:** Patient-specific `γ_bio` values (measured via functional binding assays on patient-derived cells) will predict individual treatment response with AUC > 0.80, enabling true precision dosing.

**Test:** Prospective clinical trial with patient-stratified γ_bio measurement and outcome tracking.

---

### Prediction B11: Lattice Defect Theory of Ageing

**Statement:** Biological ageing follows cumulative lattice-vacancy dynamics:

```
Fitness(t) = Fitness_0 × [1 − α × (1 − f(t/τ_lifespan))]
```

where `τ_lifespan` ≈ 85 years (human) and `α ≈ 0.3` (maximal fitness loss). This predicts that anti-ageing interventions are most effective before `t = τ_lifespan / 2` ≈ 42 years.

---

### Prediction B12: Information-Theoretic Drug Design

**Statement:** The number of bits of "therapeutic information" a drug can deliver is bounded by the protein-lattice holographic limit:

```
I_max = |Λ_protein| × ln 2  (nats)
```

For a 300-residue target: `I_max ≈ 4.28 × 0.693 ≈ 2.97 nats ≈ 4.28 bits`. This fundamental limit constrains how much biological information a single drug molecule can encode in its binding interaction.

---

## Summary Table: All Predictions Ranked by Testability

| # | Prediction | Timeframe | Key metric | Falsification criterion |
|---|---|---|---|---|
| B1 | Kinase inhibitor response time | 2026–2028 | r² > 0.60 | r² < 0.30 |
| B2 | Anti-amyloid efficacy threshold | 2026–2028 | ε < 0.20 predicts success | No ε-outcome correlation |
| B3 | Combination synergy detection | 2026–2028 | r > 0.50 for HR prediction | r < 0.20 |
| B4 | Neuroprotective dosing window | 2026–2030 | 80% benefit within t_optimal | < 50% benefit in window |
| B5 | Multi-target composite score | 2026–2030 | AUC > 0.70 for Phase II | AUC < 0.55 |
| B6 | Binding-affinity sweet spot | 2026–2030 | 70% of drugs in [0.15, 0.40] | < 40% in range |
| B7 | ε < 0.10 design constraint | 2026–2035 | 2× success rate | No improvement |
| B8 | Disease progression universality | 2026–2035 | < 10% RMS residuals | > 20% RMS |
| B9 | Biomedical Hubble constant (~8.4%) | 2026–2035 | Ceiling at ~8–9% | Many drugs exceed 15% |
| B10 | Personalised γ_bio measurement | 2035+ | AUC > 0.80 | AUC < 0.60 |
| B11 | Lattice defect theory of ageing | 2035+ | Optimal intervention age ~42 | No age dependence |
| B12 | Information-theoretic drug limit | 2035+ | 4.28-bit bound | Drugs exceed bound |

---

## How to Falsify the Biomedical PCP Framework

The framework is **wrong** if:

1. Drug efficacy shows no correlation with the verification coefficient `ξ_drug`
2. The relaxation profile `f(t)` systematically fails to fit drug-response curves
3. Combination synergy ratios do not predict clinical outcomes
4. The ~8.4% monotherapy ceiling is routinely exceeded by single-mechanism agents
5. The verification error `ε` has no predictive value for drug specificity

Any one of these outcomes would invalidate the cosmology → biology mathematical bridge.
