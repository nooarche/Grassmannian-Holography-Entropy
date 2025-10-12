# Grassmannian Holography Entropy

**Title:** *Grassmannian, Holography, Entropy: Facets and Celestial Correspondence*  
**Author:** Dr Daniel De La Harpe Golden  
**Affiliation:** Wicklow Mental Health Services / College of Psychiatrists of Ireland  
**Date:** 2025  
**License:** CC‑BY 4.0 International

---

## Abstract
We present a boundary‑first account of scattering in which positive geometry, universal soft theorems, and celestial holography are three facets of the same structure. Starting from the canonical differential logarithm form on the positive Grassmannian, we identify physical facets with soft/factorization limits of amplitudes and show how these map, under a Mellin (energy) transform, to simple poles at conformal weight Δ = 1 in celestial correlators corresponding to BMS charges. A normalized information density \(\widehat{\mathcal I}_2\) derived from the canonical form is triangulation‑invariant and stationary under spurious‑only deformations, suggesting an information‑theoretic extremality principle.

This project presents a geometric bridge between *positive geometry* in scattering amplitudes and *celestial holography* in asymptotically flat quantum gravity.  
The paper shows that the canonical differential form on the positive Grassmannian maps, under the Mellin transform, to the universal soft pole at conformal weight Δ = 1 in celestial correlators—establishing an explicit correspondence between momentum-space factorisation, boundary symmetries, and information-theoretic extremality.  

Mathematically, the treatment is fully explicit: all correspondences are worked out algebraically for the four- and five-point maximally-helicity-violating sectors, with distributional regularisation, triangulation invariance, and total-variation formalism stated precisely.  
The resulting structure defines a triangulation-invariant functional \(\widehat{\mathcal I}_2\) whose stationarity encodes the same soft-balance condition that appears as a Ward identity on the celestial sphere.

---

## What are *celestial correlators*?

Ordinary scattering amplitudes \(\mathcal A_n(p_i)\) depend on particle momenta \(p_i\).  
Celestial holography recasts them by performing a Mellin transform over each particle’s energy \(\omega_i\), producing
\[
\widetilde{\mathcal A}_n(\Delta_i,z_i,\bar z_i)
 = \int_0^\infty\!\!\prod_i d\omega_i\,\omega_i^{\Delta_i-1}
   \delta^{(4)}\!\Big(\sum_i\omega_i q_i(z_i,\bar z_i)\Big)\mathcal A_n.
\]
The transformed quantity behaves as an *n-point correlator* of conformal primary operators  
\(\mathcal O_{\Delta_i,J_i}(z_i,\bar z_i)\) on the *celestial sphere*—the sphere at null infinity of Minkowski spacetime.  
In this “celestial CFT,” soft theorems become Ward identities for asymptotic symmetries (BMS).  
A simple pole at Δ = 1 corresponds to the universal leading soft factor.  

Thus, the *celestial correlator* is a holographic rewriting of scattering data as a two-dimensional conformal correlation function, providing a natural language to compare geometric, field-theoretic, and information-theoretic structures.


---

## Citation
De La Harpe Golden, D. (2025). *Grassmannian, Holography, Entropy: Facets and Celestial Correspondence.*  
Available at [arXiv: to be assigned].

---

## Compilation
```bash
pdflatex grassmannian_holography_entropy.tex
bibtex grassmannian_holography_entropy
pdflatex grassmannian_holography_entropy.tex
pdflatex grassmannian_holography_entropy.tex
```

---

## Acknowledgments
This manuscript was prepared with assistance from the OpenAI ChatGPT system (GPT‑5) for LaTeX correction, citation integrity, and style consistency. All conceptual and theoretical content remains the author’s original work.

---

© 2025 Daniel De La Harpe Golden — Licensed under CC‑BY 4.0.
