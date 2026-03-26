# Bridge Notes: Grassmannian–Holography–Entropy ↔ Transfer Entropy (arXiv 2409.01650)

*Re-entry reference. Created 2026-03-25.*

---

## Part 1 — Where the Repo Paper Stands

**Full title:** *Grassmannian, Holography, Entropy: Facets and Celestial Correspondence*
**Author:** Daniel De La Harpe Golden (with AI collaboration)

### Core chain of correspondences

```
Gr⁺(2,n) cell
  → canonical dlog form  Ω = ⋀ dlog xᵢ
  → codimension-1 facet (cᵢ → 0)  [soft / factorization limit]
  → ω⁻¹ scaling of amplitude
  → Mellin transform  ∫ dω ω^{Δ-1} (ω⁻¹ A₃) = A₃ Γ(Δ-1)
  → simple pole at Δ = 1
  → BMS Ward identity (soft charge insertion)
```

The 4-point MHV example is worked out explicitly.

### Normalized information density

$$\widehat{\mathcal{I}}_2[\mathcal{C}] = \frac{\int_\mathcal{C} |\Omega|^2}{\left(\int_\mathcal{C} |\Omega|\right)^2}$$

- Dimensionless ratio in (0, 1], equals 1 only when Ω is perfectly uniform.
- **Triangulation-invariant**: doesn't depend on how the geometry is subdivided.
- **L² choice** is deliberate: Shannon (α=1) is trivially constant; L² is algebraically stable under rational reparametrizations.
- Used as a *diagnostic / consistency check*, not claimed as a full entropy functional.

### Central conjecture (Variational Soft Balance)

$$\delta\widehat{\mathcal{I}}_2 = 0 \quad\Longleftrightarrow\quad \nabla_\mu J^\mu_\text{soft} = 0$$

Stationarity of the information density under deformations that move only spurious (internal) boundaries is conjectured to be equivalent to soft charge conservation.

### Open questions in the paper

1. **Loop level**: extend Î₂ and the facet → pole correspondence beyond tree level.
2. **Gravity from extremality**: do perturbations away from δÎ₂ = 0 reproduce the linearized Einstein equations at null infinity?
3. **Higher multiplicity**: five-point check is sketched; general n is open.

---

## Part 2 — What the New Paper Brings

**Paper:** *Exact computation of Transfer Entropy with Path Weight Sampling*
**Authors:** Avishek Das & Pieter Rein ten Wolde (AMOLF, Amsterdam)
**arXiv:** 2409.01650v4

### Core concept: Transfer entropy

$$T_{X \to Y} = \sum_k I\!\left(X_j(k{+}1);\, X_{i[0,k]} \,\big|\, X_{j[0,k]}\right)$$

Directional, causal information flow from variable X's past trajectory to Y's future, conditioned on Y's own past. Unlike mutual information, it is *asymmetric* and detects genuine causal influence.

### TE-PWS algorithm

- Systems described by Langevin dynamics: $\dot{X} = F(t) + \xi(t)$
- Trajectory likelihoods computed via **Onsager–Machlup action** (path integral over trajectory space)
- Monte Carlo average over signal trajectories using **Rosenbluth–Rosenbluth** importance sampling
- Handles: nonlinearity, feedback loops, hidden variables, jump processes, transient dynamics
- First **exact, unbiased** method — no convergence artifacts from binning or nearest-neighbor estimation

### Key result: feedback can violate the data processing inequality

In a chain X₁ → X₂ → X₃ without feedback, the DPI gives T_{X₁→X₃} ≤ T_{X₁→X₂}.
With a feedback loop X₃ → X₁, the DPI is violated:

$$T_{X_1 \to X_3} > T_{X_1 \to X_2} \quad \text{(feedback amplification)}$$

This shows information can be "routed around" intermediaries when feedback is present.

---

## Part 3 — Conceptual Bridges

| Repo concept | PDF concept | Bridge / connection |
|---|---|---|
| Î₂ = (∫\|Ω\|²)/(∫\|Ω\|)² | Transfer entropy T_{X→Y} | Both are directed, asymmetric information measures. Î₂ measures geometric concentration; T measures causal flow |
| Canonical dlog form Ω | Path weight / Onsager–Machlup action | Both are trajectory-space integrations with weights. Ω is the "measure" on the amplitude geometry; path weights are the measure on stochastic trajectories |
| δÎ₂ = 0 (stationarity) | DPI and feedback amplification | DPI violation = information flow not in equilibrium; stationarity = information balance. These may be two languages for the same underlying principle |
| Soft charge conservation ∇·J_soft = 0 | T_{X→Y} = 0 (no information flow) | Conservation of soft charge = no net information flux across null infinity — directly analogous to vanishing transfer entropy |
| Mellin transform (energy integration) | Marginalization over hidden variables (RR scheme) | Both integrate out a variable (energy ω or hidden X_{i}) to obtain a reduced description |
| Bulk scattering → boundary correlator (holography) | T_{bulk → boundary} with hidden bulk variables | Holographic reconstruction as transfer entropy: the bulk geometry is the "hidden variable"; the celestial correlator is the observable output |
| Loop-level open question | TE-PWS is exact at all loop orders (as a stochastic method) | The path-weight technique is exact for any dynamical order. This suggests a potential route for loop-level Î₂ calculations |

---

## Part 4 — Concrete Open Questions Connecting the Two

**Q1: Can transfer entropy formalize soft charge conservation?**
The conjecture δÎ₂ = 0 ↔ ∇·J_soft = 0 is stated geometrically. Transfer entropy provides a stochastic / information-theoretic alternative: is T_{bulk→boundary} = 0 when the BMS Ward identity holds? If so, soft charge conservation is literally a statement about zero net directional information flow from bulk geometry to boundary.

**Q2: Does TE-PWS offer a computational route to Î₂ at loop level?**
The paper is stuck at tree level for Î₂. Loop amplitudes involve integration over loop momenta — a hidden variable marginalization problem. TE-PWS handles exactly this: marginalization over hidden variables via path weights. Adapting the Rosenbluth–Rosenbluth scheme to loop-momentum space could give a Monte Carlo estimator for Î₂ at one loop.

**Q3: Does feedback in the celestial picture violate the amplitude-geometry DPI?**
In the stochastic paper, feedback (X₃ → X₁) breaks the DPI and amplifies information transfer. In the holographic picture, does back-reaction (boundary → bulk) play the same role? The loop-level corrections to soft theorems could be the "feedback" that makes T_{Gr⁺ → celestial} > T_{tree level}. This would mean loop corrections are literally feedback-induced DPI violations in information-geometric terms.

**Q4: Is Î₂ a special case of a more general transfer entropy functional?**
Î₂ is built from |Ω|² normalized by |Ω|². Transfer entropy is built from ratios of conditional probabilities. Both are L²-type information ratios. Is there a unified framework — a "geometric transfer entropy" — where the canonical form plays the role of the path likelihood, and Î₂ is the zero-feedback special case of T_{bulk→boundary}?

---

## Part 5 — Candidate Citation / Connection for the Repo Paper

If Q1 or Q4 above develops into something concrete, the natural citation would be:

> A. Das and P. R. ten Wolde, "Exact computation of Transfer Entropy with Path Weight Sampling," arXiv:2409.01650 [cond-mat.stat-mech] (2024).

A note could be added to the gravity–entropy section (§5) of the paper:

*"The stationarity condition δÎ₂ = 0 has a natural interpretation in information-theoretic terms: it resembles a vanishing transfer entropy condition in the sense of [Das–ten Wolde 2024], where directional information flow is measured via path weight sampling over trajectory space. The analogy suggests that the Onsager–Machlup path integral, used there for exact transfer entropy computation, may provide a computational route to loop-level extensions of the present framework."*

---

## Quick-Reference Glossary

| Symbol | Meaning |
|---|---|
| Gr⁺(2,n) | Positive Grassmannian — the geometry |
| Ω | Canonical dlog differential form on Gr⁺(2,n) |
| Î₂[C] | Normalized information density = (∫\|Ω\|²)/(∫\|Ω\|)² |
| Δ | Conformal dimension in celestial basis (Mellin dual to energy ω) |
| BMS | Bondi–van der Burg–Metzner–Sachs asymptotic symmetry group |
| T_{X→Y} | Transfer entropy — directional information flow (Das–ten Wolde) |
| TE-PWS | Transfer Entropy via Path Weight Sampling algorithm |
| DPI | Data Processing Inequality: T_{X→Z} ≤ min(T_{X→Y}, T_{Y→Z}) in chains |
| Onsager–Machlup | Path integral weight for Langevin trajectories |
