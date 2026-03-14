# ToAEx-001-v02 - Galactic Rotation as Fisher-Geometric Smoothing of Mass Distributions

**Author:** Pedro R. Andrade\
**Date:** 13MAR2026\
**DOI:** [10.5281/zenodo.17166444]\
**Status:** Experimental design\
**Document Name:** _ToAEx-001-v02 - Galactic Rotation via Informational Smoothing.md_


***

# Abstract

Within the framework of the Theory of Absolutely Everything (ToAE), physical systems evolve by minimizing the informational functional

$$\
J[\psi;\phi]
=\
S[\rho]\
+\
\lambda R_{\mathrm{coh}}\
+\
\gamma I_F\
$$

where $S$ is entropy, $R_{\text{coh}}$ measures coherence relative to a reference frame, and $I_F$ is Fisher information.

Recent work shows that the Fisher term introduces a natural differential operator

$$\
\nabla^2 \log\rho\
$$

when the functional is varied. This operator acts as an informational curvature term that smooths density gradients.

When applied to baryonic mass distributions in galaxies, this term produces an additional acceleration component that modifies Newtonian gravity. The resulting dynamics naturally generates flat galactic rotation curves without requiring non-baryonic dark matter halos.

This document presents the derivation of this correction and outlines observational tests.

***

## 1. Informational Dynamics in the ToAE

The ToAE framework models physical evolution as the minimization of the informational functional

$$\
J[\psi;\phi]
=\
S[\rho]\
+\
\lambda R_{\mathrm{coh}}\
+\
\gamma I_F\
$$
where

* $S[\rho]$ measures informational entropy

* $R_{\text{coh}}$ measures coherence between system and reference frame

* $I_F$ is Fisher information.

The Fisher term acts as a regularization penalty that discourages unstable informational configurations.

For spatial density fields, Fisher information takes the form

$$\
I_F
=\
\int\
\rho(x)|\nabla \log \rho(x)|^2\
dx\
$$

which measures the sharpness of density gradients.

***

## 2. Variational Derivation of the Fisher Operator

To determine the physical consequences of the Fisher term we compute the functional derivative.

Rewriting the functional,

$$\
I_F
=\
\int\
\frac{|\nabla \rho|^2}{\rho}\
dx\
$$

Applying the Euler–Lagrange variation gives

$$\
\frac{\delta I_F}{\delta\rho}
=\
-\frac{2\nabla^2\rho}{\rho}\
+\
\frac{|\nabla\rho|^2}{\rho^2}.\
$$

Using the identity

$$\
\nabla^2\log\rho
=\
\frac{\nabla^2\rho}{\rho} -
\frac{|\nabla\rho|^2}{\rho^2},\
$$
the variation can be rewriten as

$$\
\frac{\delta I_F}{\delta\rho}
=\
-2\nabla^2 \log\rho\
-\
\frac{|\nabla\rho|^2}{\rho^2}.\
$$

The dominant term for smooth density variations is the linear operator $-\nabla^2\log\rho$, which drives the system toward configurations with minimal logarithmic curvature.

***

## 3. Informational Potential

Within the ToAE functional, this variation introduces an effective informational potential

$$\
V_{\mathrm{info}}
=\
\gamma\
\nabla^2\
\log\rho\
$$

The corresponding acceleration is

$$\
a_{\mathrm{info}}
=\
-\nabla V_{\mathrm{info}}\
$$

which yields

$$\
a_{\mathrm{info}}\
\propto\
\nabla(\nabla^2\log\rho)\
$$

This term represents an informational curvature force that acts to stabilize density distributions.

***

## 4. Application to Galactic Mass Distributions

Consider a galaxy with baryonic density

$$\
\rho_b(r)\
$$

The informational acceleration becomes

$$\
a_{\mathrm{info}}(r)
=\
K\
\frac{d}{dr}\
\left(\
\nabla^2\
\log\rho_b(r)\
\right)\
$$

where $K$ is a universal coupling constant determined by the weight of the Fisher term in the ToAE functional.

The total radial acceleration becomes

$$\
a(r)
=\
a_{\text{Newton}}\
+\
a_{\text{info}}\
$$

with

$$\
a_{\text{Newton}}
=\
\frac{GM_b(r)}{r^2}\
$$

***

## 5. Modified Rotation Curve

The circular velocity is therefore

$$\
v_c^2(r)
=\
\frac{GM_b(r)}{r}\
+\
r a_{\mathrm{info}}(r)\
$$

The informational term becomes significant at large radii where density gradients become shallow.

This naturally produces flattened rotation curves.

***

## 6. Scaling with Information Content

The strength of the informational correction depends on the total informational complexity of the baryonic system.

For a galaxy with baryonic mass $M_b$, the number of microscopic degrees of freedom is approximately

$$\
N \sim \frac{M_b}{m_p}\
$$

Information scales as

$$\
I \sim \log N\
$$

Thus the effective coupling becomes

$$\
K\
\sim\
\kappa\
\log\left(\frac{M_b}{m_p}\right)\
$$

And the informational acceleration

$$
a_{\text{info}}(r) = \kappa \cdot \log\left(\frac{M_b}{m_p}\right) \cdot \nabla(\nabla^2 \log \rho_b(r))
$$

This scaling links the informational correction directly to baryonic matter.

***

## 7. Observational Predictions

The model predicts:

1. Flat galactic rotation curves.

2. A correlation between baryonic mass and asymptotic velocity.

3. A universal coupling constant $\kappa$ across galaxies.

These predictions can be tested using observational datasets such as the SPARC galaxy catalog.

***

## 8. Order-of-Magnitude Estimate

To evaluate the plausibility of the informational correction, we can perform an order-of-magnitude estimate for a typical galaxy such as the Milky Way.

Consider a baryonic mass

$$\
M_b \sim 10^{11} M_\odot\
$$

and a characteristic disk scale length

$$\
R_d \sim 4,\text{kpc}.\
$$

The approximate number of microscopic constituents is

$$\
N \sim \frac{M_b}{m_p},\
$$

which yields

$$\
\log\left(\frac{M_b}{m_p}\right) \approx 160 .\
$$

To estimate the geometric operator

$$\
\nabla(\nabla^2 \log \rho_b),\
$$

assume an exponential disk density profile

$$\
\rho_b(r) \propto e^{-r/R_d}.\
$$

For such a profile,

$$\
\nabla(\nabla^2 \log \rho_b)\
\sim\
\frac{2}{r^2 R_d}.\
$$

Evaluating this expression at a characteristic radius $r \sim R_d$ gives approximately

$$\
\nabla(\nabla^2 \log \rho_b)\
\sim\
10^{-60},\text{m}^{-3}.\
$$

The informational acceleration predicted by the model is

$$\
a_{\text{info}}
=\
\kappa\
\log\left(\frac{M_b}{m_p}\right)\
\nabla(\nabla^2 \log \rho_b).\
$$

For this term to be comparable to the observed centripetal acceleration in the outer regions of galactic disks,

$$\
\frac{v^2}{r}\
\sim\
10^{-10} \text{m/s}^2\
\quad\
(r \sim 8 \text{kpc}),\
$$

the coupling constant must be approximately

$$\
\kappa\
\sim\
10^{47}\
\text{m}^4/\text{s}^2.\
$$

Although numerically large, this value is not excluded by any known physical constraint. It should therefore be regarded as an effective parameter to be determined empirically, for example through fitting galactic rotation curves in observational datasets such as the SPARC galaxy catalog.

***

## 9. Interpretation

In the ToAE framework, the additional acceleration arises from the geometry of the information manifold rather than from unseen mass.

Galactic systems evolve toward configurations that minimize informational curvature.

The resulting smoothing dynamics produces a modification of gravitational behavior at large scales.

Thus the apparent effects attributed to dark matter may reflect the informational structure of baryonic matter distributions.

***
## 10. References

R. Andrade, P. (2025). Theory of Absolutely Everything - A blueprint to renew human knowledge (19SEP2025). Zenodo. [https://doi.org/10.5281/zenodo.17162302]

R. Andrade, P. (2025). ToAEx-0: Experimental Framework for the Theory of Absolutely Everything (20SEP2025). Zenodo. [https://doi.org/10.5281/zenodo.17166248]

---

This document was produced and refined with the help of artificial intelligence.

This document and its listed documents can be accessed at [https://github.com/pedrora/Theory-of-Absolutely-Everything].

All documents of this theory are released under the _Creative Commons Zero v1.0 Universal_ license and are public domain.
