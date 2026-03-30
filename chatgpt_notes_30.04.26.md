# Reviewer-style notes on strengthening the paper

These comments are offered in a constructive spirit. The paper has a strong conceptual core and a distinctive synthesis: positive geometry, soft/factorization structure, celestial Mellin poles, and an information-balance functional are brought into a single frame. The central intuition is compelling. The main task now is to sharpen which claims are already established, which are plausible conjectures, and which currently overreach the available formalism.

---

## Overall assessment

The paper is strongest when it does the following:

1. Gives an explicit tree-level chain from facet of positive geometry to soft scaling to Mellin pole at \(\Delta=1\) to Bondi–van der Burg–Metzner–Sachs (BMS) Ward identity.
2. Introduces \(\widehat{\mathcal I}_2\) as a triangulation-invariant diagnostic built from the canonical form.
3. Suggests that stationarity of this functional under spurious-only deformations may encode a deeper balance principle.

The paper becomes less secure when it moves too quickly from:
- diagnostic \(\widehat{\mathcal I}_2\),
to
- entropy in a full physical sense,
to
- gravitational dynamics,
to
- directional information flow.

The main recommendation is therefore to **preserve the boldness of the vision while improving the hierarchy of claims**.

---

## Major recommendation: introduce a three-tier claim structure

I strongly recommend explicitly dividing statements into three categories throughout the introduction, gravity/entropy section, and conclusion:

### Tier 1 — established in the present paper
Claims actually demonstrated at tree level.

Examples:
- A physical codimension-one facet producing \(\omega^{-1}\) soft scaling Mellin-maps to a simple pole at \(\Delta=1\).
- The four-point maximally helicity-violating (MHV) example is worked out explicitly.
- \(\widehat{\mathcal I}_2\) is proposed as a triangulation-invariant \(L^2\)-based diagnostic and shown numerically to be stable under retriangulation / spurious-only deformations in the examples considered.

### Tier 2 — motivated conjectures
Claims that are plausible extensions of the formalism, but not yet derived.

Examples:
- \(\delta \widehat{\mathcal I}_2 = 0 \Longleftrightarrow \nabla_\mu J^\mu_{\text{soft}}=0\).
- The suggestion that perturbations away from stationarity may encode gravitational response.
- The idea that loop-level corrections may be understood as corrections to an information-balance law.

### Tier 3 — broader interpretive speculation
Conceptual framing that is suggestive, but not yet formal.

Examples:
- Gravity as an extremal information-preserving projection of amplitude geometry.
- A full equivalence between soft charge conservation and a directional information-flow statement.
- A transfer-entropy or thermodynamic-gravity reading of the framework.

This tiering would make the paper much more robust and reviewer-proof.

---

## Strengths that should be preserved and foregrounded

### 1. The facet \(\to\) pole map is clear and distinctive
This is the strongest concrete contribution. It should remain the center of gravity of the paper. The paper is at its best when it stays close to the explicit chain:

\[
\text{facet}
\to
\omega^{-1}
\to
\Gamma(\Delta-1)
\to
(\Delta-1)^{-1}
\to
\text{Ward identity}
\]

That chain is elegant, intelligible, and mathematically crisp.

### 2. The use of \(\widehat{\mathcal I}_2\) as a diagnostic is interesting
The paper is persuasive when \(\widehat{\mathcal I}_2\) is treated as:
- a triangulation-invariant consistency check,
- a measure of concentration / uniformity of the canonical density,
- and a possible indicator of stationarity.

It is less persuasive when \(\widehat{\mathcal I}_2\) is treated too quickly as a full entropy functional.

### 3. The boundary-first viewpoint is coherent
The framing in which bulk positive geometry, soft structure, and celestial boundary insertions are different facets of one structure is the genuine conceptual contribution here. This is worth emphasizing clearly and repeatedly.

---

## Where the paper currently overstates things

### 1. \(\widehat{\mathcal I}_2\) is not yet obviously a directional information measure
At present,
\[
\widehat{\mathcal I}_2[\mathcal C]
=
\frac{\int_{\mathcal C} |\Omega|^2}{\left(\int_{\mathcal C} |\Omega|\right)^2}
\]
is a normalized concentration / uniformity diagnostic on a geometry.

This does **not yet** make it formally analogous to transfer entropy, which is explicitly:
- directional,
- conditional,
- and causal / time-ordered.

Recommendation:
state clearly that \(\widehat{\mathcal I}_2\) is currently a **geometric information functional**, not yet a directional transfer-entropy functional. If desired, introduce the notion that a directional generalization may exist, but distinguish it from the present object.

### 2. “Entropy” language should be tightened
The current text sometimes moves from “information density diagnostic” to “entropy” too quickly.

Recommendation:
use language such as:
- “entropy-like diagnostic,”
- “information-balance functional,”
- “concentration functional,”
- “candidate extremality functional,”

unless or until a stronger axiomatic entropy interpretation is given.

### 3. Conservation does not imply zero information flow
If the paper or future notes suggest that soft charge conservation is equivalent to vanishing transfer entropy, this should be softened.

A conservation law usually means a **balanced net flux**, not necessarily zero directional flow. There can be nonzero directional transfer with overall conservation.

Recommendation:
phrase this instead as:
> soft charge conservation may correspond to a balance condition on net directional information flux across null infinity, rather than the literal absence of directional information flow.

---

## Recommendations on the transfer entropy bridge

The transfer entropy bridge is promising, but needs careful framing.

### What is genuinely promising
The strongest points of contact are:

#### A. Hidden-variable marginalization
This is perhaps the most fertile bridge.

- In the paper, Mellin transform integrates over energy.
- At loop level, one would integrate over loop variables / hidden geometric degrees of freedom.
- In transfer entropy with path-weight sampling, one integrates over hidden trajectory variables to obtain directional information flow.

This analogy is strong and worth developing.

#### B. Directional projection from geometry to boundary
The paper already has a directionality of interpretation:
- positive geometry / canonical form,
- soft/facet residue,
- Mellin transform,
- celestial correlator / boundary Ward identity.

Transfer entropy may therefore be a useful future language for the **projection** from geometric data to boundary observables.

#### C. Feedback as an analogy for backreaction
The analogy between feedback in transfer entropy systems and loop/backreaction effects in celestial / holographic settings is suggestive.

However, it should be phrased as an analogy or heuristic, not a theorem.

### What should be softened
I recommend avoiding statements of the following strong type:
- “\(\widehat{\mathcal I}_2\) and transfer entropy are both directed asymmetric measures.”
- “soft charge conservation is literally zero transfer entropy.”
- “path-weight sampling provides an exact loop-level solution for the present framework.”

These are too strong as presently formulated.

### Suggested replacement language
A safer formulation would be:

> Transfer entropy is not identified here with \(\widehat{\mathcal I}_2\). Rather, it provides a useful conceptual and possibly computational language for directional information flow under hidden-variable marginalization. This suggests a possible route for extending the present tree-level geometric information functional to a directional, loop-sensitive framework.

That keeps the bridge alive without overcommitting.

---

## Recommendations on the gravity / thermodynamic interpretation

The thermodynamic / emergent gravity reading is one of the most interesting parts of the paper, but it needs a clearer status.

### What works well
The paper already has the structure of a balance-law picture:
- a bulk geometric measure,
- a boundary conservation law,
- a stationarity principle,
- and a suggestion that physically meaningful dynamics may emerge from extremality.

That is genuinely close in spirit to emergent gravity programs.

### What would strengthen it
It would help to say explicitly that the paper is **not deriving Einstein equations**, but rather proposing a structural analogy:

- canonical-form balance in positive geometry,
- Mellin projection to boundary current conservation,
- candidate information-extremality principle,
- possible future gravitational interpretation.

### Suggested phrasing
> The present results do not derive gravitational field equations. Rather, they suggest that the geometry-to-celestial map may admit a thermodynamic interpretation in which boundary symmetry conservation corresponds to stationarity of a bulk information functional.

That would make the paper much more defensible.

---

## Quadratic / higher-curvature gravity: how to connect without overstating

If the paper or future notes want to connect this framework to higher-curvature or quadratic gravity, the cleanest way is the following:

1. Einstein gravity can be viewed, in emergent thermodynamic approaches, as a leading-order equation of state.
2. Higher-curvature terms correspond to corrected entropy / corrected response laws.
3. Therefore, if the current tree-level \(\widehat{\mathcal I}_2\) balance principle is a leading-order information law, then loop-level or feedback-corrected versions of it may be expected to correspond, on the gravity side, to corrected effective dynamics analogous to higher-curvature gravity.

This is a good conceptual bridge.

What should be avoided is any implication that the present manuscript already derives curvature-squared dynamics.

A safe way to phrase it:
> If the tree-level stationarity of \(\widehat{\mathcal I}_2\) is interpreted as a leading-order balance law, then departures from this regime may naturally be expected to correspond, on the gravitational side, to corrected effective dynamics analogous to higher-curvature response terms.

---

## Concrete revision suggestions by section

### Introduction
Recommendation:
add a short paragraph distinguishing:
- proven tree-level correspondence,
- conjectured extremality principle,
- broader gravity / information interpretation.

This would immediately orient the reader and prevent confusion.

### Related Work and Positioning
Recommendation:
situate the work more explicitly relative to:
- celestial holography,
- positive geometry / canonical forms,
- soft theorem / Ward identity literature,
- information-theoretic interpretations,
- and emergent gravity analogies.

State clearly that the paper’s distinct contribution is **not** a general reformulation of entropy in scattering, but a specific tree-level facet-to-pole map plus a proposed geometric diagnostic.

### Normalized Information Density and Extremality
Recommendation:
tighten the interpretation of \(\widehat{\mathcal I}_2\).

Possible phrasing:
- “diagnostic of concentration / uniformity,”
- “triangulation-invariant \(L^2\) functional,”
- “entropy-like but not yet an axiomatic entropy.”

Also state more clearly which parts are proven and which are numerically observed.

### Gravity and Entropy section
Recommendation:
this section needs the most careful tightening.

Suggested structure:
1. Restate the established tree-level correspondence.
2. Introduce the variational soft balance as a conjecture.
3. Present the gravity / thermodynamic reading as an interpretation, not a derivation.
4. Explicitly list the missing steps needed before any claim about Einstein dynamics or loop-corrected gravitational equations could be made.

This would substantially improve credibility.

### Conclusion
Recommendation:
end with a precise statement of what has been achieved:
- explicit tree-level facet-to-pole correspondence,
- diagnostic \(\widehat{\mathcal I}_2\),
- conjectural extremality / soft-balance relation,
- roadmap toward loop-level, directional-information, and emergent-gravity extensions.

---

## Specific formulation improvements

### Instead of:
“Both viewpoints therefore describe the redistribution—but not the loss—of geometric information.”

Consider:
> Both viewpoints suggest a residue- or charge-balanced redistribution of the relevant geometric data, though the precise information-theoretic meaning of this balance remains to be formalized.

### Instead of:
“gravitational dynamics may arise from the requirement that the holographic projection of amplitude geometry extremizes a global information functional”

Consider:
> the present tree-level correspondence motivates the conjecture that aspects of gravitational dynamics may eventually be expressible as extremality conditions on a suitable information functional associated with amplitude geometry.

### Instead of:
“\(\widehat{\mathcal I}_2\) behaves as an entropy-like quantity”

Consider:
> \(\widehat{\mathcal I}_2\) behaves as an entropy-like concentration functional in the limited sense that stationarity corresponds to a balanced distribution of canonical measure under the class of deformations considered.

### Instead of:
“soft charge conservation is an entropy balance equation”

Consider:
> soft charge conservation invites comparison with an entropy- or information-balance law, though the present paper does not yet establish a full thermodynamic derivation.

---

## A useful table to add to the manuscript or notes

| Status | Claim |
|---|---|
| Established | Physical soft facet \(\to\) \(\omega^{-1}\) scaling \(\to\) Mellin pole at \(\Delta=1\) |
| Established / numerical | \(\widehat{\mathcal I}_2\) is triangulation-stable in tested examples |
| Conjectural | \(\delta \widehat{\mathcal I}_2 = 0 \Longleftrightarrow \nabla_\mu J^\mu_{\text{soft}}=0\) |
| Interpretive | \(\widehat{\mathcal I}_2\) as an information-balance / entropy-like functional |
| Speculative extension | Loop corrections / backreaction as non-equilibrium or feedback corrections |
| Speculative extension | Relationship to emergent thermodynamic gravity and higher-curvature response |

This would help readers and reviewers enormously.

---

## Most promising future directions

The most promising next developments seem to be:

1. **Formalize the deformation class** for which \(\delta \widehat{\mathcal I}_2\) is being taken.
2. **Clarify regulator dependence** of the functional and of the variational statement.
3. **Construct a directional generalization** of \(\widehat{\mathcal I}_2\) if transfer entropy is to become more than analogy.
4. **Investigate loop-level hidden-variable marginalization** in a way that does not overclaim but does connect naturally to the Mellin / projection picture.
5. **Separate tree-level theorem from gravity-level speculation** more cleanly.

---

## Bottom-line reviewer summary

This is an imaginative and potentially important paper. Its most persuasive contribution is the explicit tree-level correspondence between positive-geometry facets and celestial \(\Delta=1\) poles, together with the proposal of a triangulation-invariant geometric information diagnostic. The main revisions needed are not to reduce ambition, but to improve claim discipline: distinguish demonstrated results from conjectures and broader interpretive speculation; tighten the meaning of \(\widehat{\mathcal I}_2\); and present the gravity / transfer-entropy connections as promising extensions rather than already-established equivalences.

With that tightening, the paper would become substantially stronger, clearer, and more resilient to critical review.