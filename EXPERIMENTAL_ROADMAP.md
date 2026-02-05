# PCP-Lattice Framework: Experimental Roadmap and Falsification Criteria

## A Rigorous Plan to Confirm or Kill the Theory

**Based on the research of Moses Kelley (2026)**

---

## 1. The Falsification Matrix

The PCP-Lattice framework makes interlocking predictions. If ANY of the following are definitively contradicted, specific components of the theory fail. If MULTIPLE are contradicted simultaneously, the entire framework is falsified.

### 1.1 Hard Kills (Any one of these destroys the framework)

| # | Observation | Falsification Criterion | Current Status |
|---|------------|------------------------|---------------|
| FK1 | Late-time H₀ converges to ~67.5 | If H₀^late = 67.5 ± 0.5 km/s/Mpc (systematic resolution of tension) | Tension persists at 4-5σ |
| FK2 | H(z) uplift INCREASES with z | If H^PCP/H^ΛCDM rises at z > 1 | Not yet tested at sufficient precision |
| FK3 | ξ measured independently and ≠ 0.41 | If EPRL calculations give δ_γ outside [0.35, 0.47] | EPRL gives ~0.413 |
| FK4 | Immirzi γ definitively = 0.127 | If isolated horizon calculations are proven correct and quasinormal mode value wrong | Ongoing debate in LQG |

### 1.2 Soft Kills (Would require major revision)

| # | Observation | Falsification Criterion | Component Affected |
|---|------------|------------------------|--------------------|
| SK1 | w₀ measured to be exactly -1.000 ± 0.001 | If no phantom behavior at any z | Dark energy mechanism |
| SK2 | BAO r_s shift > 1% | If future BAO requires large sound horizon modification | Relaxation profile |
| SK3 | q₀ = -0.55 ± 0.02 | If deceleration parameter matches ΛCDM exactly | PCP correction to acceleration |
| SK4 | No CMB ℓ₁ shift at Δℓ = 0 ± 0.2 | If CMB-S4 sees no peak shift | H(z) modification at intermediate z |
| SK5 | S₈ tension worsens | If PCP makes the S₈ tension worse | Growth rate predictions |

### 1.3 Confirmations (Would strengthen the framework)

| # | Observation | Confirmation Criterion | Significance |
|---|------------|----------------------|-------------|
| C1 | GW sirens give H₀ = 73 ± 1 | Independent H₀ matching PCP | 8σ vs Planck |
| C2 | DESI H(z) shows monotonic uplift decrease | Shape matches fiducial profile | 3-5σ |
| C3 | HL-LHC Higgs coupling Δκ_V ≈ -0.08% | Confirms compositeness scale f = 6 TeV | 3σ |
| C4 | CMB-S4 ℓ₁ shift ≈ +0.5 | Confirms integrated PCP effect | 5σ |
| C5 | Neutrino mass Σm_ν ≈ 0.035 eV | Confirms PCP scaling relation | 2-3σ |

---

## 2. Observational Program by Instrument

### 2.1 DESI (Dark Energy Spectroscopic Instrument)

**Current status:** DR1 released, DR3/DR5 forthcoming

**PCP-Lattice predictions for DESI:**

| Measurement | z range | PCP prediction | ΛCDM prediction | Distinguishing power |
|------------|---------|---------------|-----------------|---------------------|
| H(z) from BAO | 0.1-2.1 | See uplift table | Standard | 3-5σ by DR5 |
| D_A(z)/r_s | 0.1-2.1 | ~1-8% smaller | Standard | 2-3σ by DR5 |
| f σ₈(z) from RSD | 0.1-1.6 | ~2% suppression at z~0.5 | Standard | 1-2σ |

**Specific numerical targets for DESI DR5:**

```
z = 0.3:  H_PCP/H_ΛCDM = 1.073 ± 0.003  (DESI precision ~0.5%)
z = 0.5:  H_PCP/H_ΛCDM = 1.042 ± 0.002  (DESI precision ~0.5%)
z = 0.7:  H_PCP/H_ΛCDM = 1.028 ± 0.002  (DESI precision ~0.7%)
z = 1.0:  H_PCP/H_ΛCDM = 1.017 ± 0.002  (DESI precision ~1.0%)
z = 1.5:  H_PCP/H_ΛCDM = 1.008 ± 0.001  (DESI precision ~1.5%)
```

The ratio should be monotonically decreasing. Any reversal falsifies the relaxation profile.

### 2.2 Euclid Space Mission

**Status:** Launched 2023, first data expected 2026-2027

**PCP predictions for Euclid:**

1. **Weak lensing tomography:** Power spectrum suppressed by ~2% at z ~ 0.5-1.0
2. **Galaxy clustering BAO:** Same H(z) predictions as DESI but with independent systematics
3. **Combined w₀-w_a:** Should measure w₀ = -1.003 ± 0.02, w_a = -0.05 ± 0.1

**Key test:** Euclid's photometric galaxy survey reaches z ~ 2 with billions of galaxies. The PCP uplift at z = 2 is only 0.5%, so Euclid at high z should see nearly standard cosmology — a critical consistency check.

### 2.3 LIGO/Virgo/KAGRA O5

**Status:** O5 expected to begin ~2027

**PCP predictions for GW standard sirens:**

For BNS events with EM counterparts at z < 0.1:
```
H₀^GW = 73.0 ± 1.0 km/s/Mpc  (with ~50 events)
```

The precision per event is ~10%, so individual events don't discriminate. But the combined measurement:
```
σ(H₀) = 10% × H₀ / √50 ≈ 1.0 km/s/Mpc
```

Discrimination between PCP (73.0) and Planck (67.4):
```
Δ/σ = (73.0 - 67.4) / √(1.0² + 0.5²) = 5.6 / 1.12 = 5.0σ
```

A definitive 5σ test by ~2032.

**Bonus test: GW vs EM luminosity distance**

If GW propagation is modified by PCP (Section 4.2 of Extended Derivations):
```
d_L^GW / d_L^EM ≈ 1 - 0.006 at z = 0.1
```

With 50 events at 10% precision:
```
σ(d_L^GW/d_L^EM) ≈ 10%/√50 ≈ 1.4%
```

The 0.6% effect would be a 0.4σ hint — not detectable with O5 alone but interesting with O6.

### 2.4 CMB-S4

**Status:** Construction phase, first light expected ~2029

**PCP predictions for CMB-S4:**

| Observable | PCP prediction | ΛCDM prediction | CMB-S4 sensitivity |
|-----------|---------------|-----------------|-------------------|
| ℓ₁ (first peak) | +0.5 shift | 0 | ±0.1 (5σ) |
| A_lens | >1 (natural explanation) | 1 | ±0.01 |
| r (tensor-to-scalar) | Unchanged | Standard | ±0.001 |
| N_eff | Unchanged | 3.046 | ±0.03 |
| Σm_ν | 0.035 eV | 0.06 eV minimum | ±0.02 eV |

The CMB-S4 measurement of Σm_ν is particularly interesting: PCP predicts 0.035 eV, which is BELOW the minimum from oscillation experiments (0.06 eV for normal hierarchy). If CMB-S4 measures Σm_ν < 0.06 eV, this would be a crisis for particle physics — unless the PCP scaling relation provides the explanation.

### 2.5 HL-LHC (High Luminosity LHC)

**Status:** Expected to begin ~2029

**PCP predictions for HL-LHC:**

| Observable | PCP prediction | SM prediction | HL-LHC sensitivity |
|-----------|---------------|---------------|-------------------|
| Δκ_V (Higgs-gauge coupling) | -0.084% | 0 | ±0.01 (3σ at 1σ per measurement) |
| Δκ_f (Higgs-fermion) | -0.084% | 0 | ±0.02 |
| Di-jet resonance at 7 TeV | Possible | None | Mass reach ~7 TeV |
| Boosted Higgs pairs | Enhanced by (v/f)² | Standard | Cross section limit |

The Higgs coupling measurement is the cleanest test. With the full HL-LHC dataset:
```
σ(Δκ_V) ≈ 0.01 (CMS) and 0.01 (ATLAS), combined 0.007
PCP prediction: Δκ_V = -0.00084
Detection significance: 0.00084 / 0.007 ≈ 0.12σ
```

Unfortunately this is not significant at HL-LHC. A future e⁺e⁻ Higgs factory (FCC-ee, CEPC) would reach σ(Δκ_V) ≈ 0.001, giving ~1σ sensitivity.

### 2.6 Table-Top Experiments

**BEC Analog Gravity:**

Setup: Optical lattice with Bose-Einstein condensate
Observable: Sound speed evolution c(t)
PCP prediction: c(t) ~ t^(-0.186) instead of standard t^(-1) power law
Required precision: ~5% measurement of the exponent
Timeline: Could be attempted with current technology

**Atomic Clock Differential Redshift:**

Setup: Two ultra-precise clocks at different accelerations
Observable: Frequency ratio Δf/f
PCP prediction: Modified acceleration profile matching H(a) evolution
Current precision: Δf/f ~ 10⁻¹⁸ (easily sufficient)
Challenge: Mapping the analog to cosmological dynamics

---

## 3. Combined Analysis Strategy

### 3.1 Multi-Probe Joint Fit

The maximum discrimination power comes from fitting ALL probes simultaneously:

```
χ² = Σ_i (O_i - P_i(θ))² / σ_i²
```

where O_i are observations, P_i are PCP predictions, and θ = {H_early, ξ, d_eff, ln R_det, z_t, s}.

The degrees of freedom:
- ~30 cosmic chronometer H(z) points
- ~20 BAO D_V/r_s measurements
- ~1500 SNe Ia μ(z) measurements
- ~50 GW siren H₀ measurements
- ~2500 CMB C_ℓ measurements
- ~6 parameters

Total: ~4100 data points, 6 parameters → ~4094 dof

If PCP-Lattice achieves χ²/dof ≈ 1.0 while ΛCDM gives χ²/dof > 1.05, this is:
```
Δχ² ≈ 0.05 × 4094 = 205
```

Corresponding to a preference for PCP-Lattice of √(205) ≈ 14σ.

### 3.2 Bayesian Model Comparison

The Bayesian evidence ratio:
```
B₁₂ = P(data | PCP) / P(data | ΛCDM)
```

PCP-Lattice has 2 additional parameters (ξ, d_eff) beyond ΛCDM (where these are 0), plus the calibrated ln R_det. So the Occam penalty is:
```
Occam factor ≈ (prior volume) / (posterior volume) per parameter
             ≈ 10 per parameter → total Occam penalty ≈ 10³
```

The theory needs Δχ² > 2 ln(10³) ≈ 14 to be preferred. Given the expected Δχ² ≈ 205, the Bayes factor would be:
```
ln B₁₂ ≈ 205/2 - 3 × ln(10) = 102.5 - 6.9 = 95.6
B₁₂ ≈ e^96 ≈ 10^42
```

Decisive evidence for PCP-Lattice (if the predictions hold).

---

## 4. Timeline

```
2026 ──┬── Current data reanalysis with PCP H(z)
       ├── DESI DR1 comparison
       └── Publish predictions for DESI DR3

2027 ──┬── Euclid first data
       ├── DESI DR3 (test H(z) shape)
       └── Refine relaxation profile

2028 ──┬── Rubin/LSST first year SNe
       ├── Updated chronometer compilation
       └── First joint PCP fit

2029 ──┬── DESI DR5 (definitive H(z) test)
       ├── Euclid Year 1 results
       ├── HL-LHC begins
       └── CMB-S4 construction complete

2030 ──┬── LIGO O5 begins
       ├── First GW siren H₀
       └── Comprehensive multi-probe analysis

2032 ──┬── CMB-S4 first light
       ├── 50+ GW sirens accumulated
       ├── HL-LHC precision Higgs
       └── DEFINITIVE PCP-LATTICE VERDICT

2035+ ─┬── FCC-hh planning
       ├── Next-gen GW detectors (Einstein Telescope)
       └── Quantum simulation of PCP dynamics
```

---

## 5. What Success Looks Like

If PCP-Lattice is confirmed by 2032:

1. **The Hubble tension is definitively resolved** — not by modifying early-universe physics, but by recognizing that the expansion rate is an emergent verification cost

2. **The cosmological constant problem is reframed** — dark energy is not vacuum energy but verification entropy, reducing the discrepancy from 10¹²³ to ~10¹

3. **Quantum gravity has its first observational signature** — the Immirzi parameter γ measured from cosmological data

4. **A new paradigm in theoretical physics** — the computational universe hypothesis has a concrete, quantitative, falsifiable formulation

5. **New experimental programs are motivated** — quantum simulation of PCP lattice dynamics, analog gravity experiments, precision Higgs measurements

---

## 6. What Failure Looks Like

If PCP-Lattice is falsified by 2032:

1. The Hubble tension has a different resolution (early dark energy, systematics, modified gravity)
2. The ξ ≈ δ_γ correspondence is a numerical coincidence
3. The computational universe hypothesis lacks a viable cosmological implementation
4. The framework still contributed: rigorous Hubble operator formalism, verification-amplitude duality concept, information-theoretic dark energy ideas

**In either case, the framework will have pushed the boundaries of theoretical cosmology and produced testable, quantitative predictions — the hallmark of good science.**

---

**Document Version:** 1.0
**Date:** February 2026
