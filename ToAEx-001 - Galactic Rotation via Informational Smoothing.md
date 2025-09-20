# ToAEx-001 - Galactic Rotation via Informational Smoothing

**Author:** Pedro R. Andrade
**Date:** 20SEP2025
**DOI:** [10.5281/zenodo.17166445]
**Status:** In design
**Requires:** Astrophysicists with access to data and computational power
**Document Name:** _ToAEx - 01 - Galactic Rotation via Informational Smoothing - proposal.md_

---

## Key technical information

This document is named ToAEx as in Experimental eXtension of the theory, providing a scientific test to the Theory of Absolutely Everything (ToAE). At the current date the ToAE is just too big and too young after its release to have any tests already performed, and there is absolutely no way to foreview a valid tracking system. It could potentially end with just the hypothesis formulated on this paper, though I am sure that it will pass, as it will pass all others tests, because they all make sense to me, otherwise I wouldn't have created this theory, so big and so wide, that explains so much. But it must also grow tall, and that can only be achieved with the labor of verifying it.

I get ahead of my self. I a theory that explains everything, this section explains the following:

- Prefix ToAEx must be used for all experiment proposals hosted on the ToAE's GitHub repository;
- The unique identifier used is the DOI number of the experimental results, final or intermediary;
- A DOI can be assigned at any experimental stage if the lead investigator deems it fit;
- ToAEx tests should be updated in the 'ToAE - Experimental avenues.md' file

## Introduction

The ToAE predicts that dark matter is an emergent phenomenon arising from the `fractalof` functional minimization, specifically from the Fisher information term $\gamma I_F$, where $\gamma$ scales with the informational complexity of the system. For galaxies, this translates to an effective acceleration term that modifies the circular velocity curve. Below is the mathematical framework to test this prediction using observed galactic rotation curves.

#### Key Equations

1. **Modified Circular Velocity**:
   The circular velocity $v_c(r)$ at radius $r$ is given by:
   $$v_c^2(r) = \frac{G M_b(r)}{r} + r \, a_{\text{info}}(r)$$
   where:
   - $G$ is the gravitational constant,
   - $M_b(r)$ is the baryonic mass within radius $r$,
   - $a_{\text{info}}(r)$ is the acceleration due to the information term.

2. **Information Acceleration**:
   $$a_{\text{info}}(r) = K \, \log\left( \frac{M_b}{m_p} \right) \, \frac{\partial}{\partial r} \left( \nabla^2 \log \rho_b(r) \right)$$
   where:
   - $K$ is a universal constant (units: $\text{m}^4 / \text{s}^2$),
   - $M_b$ is the total baryonic mass of the galaxy,
   - $m_p$ is the proton mass (approximately $1.67 \times 10^{-27} \, \text{kg}$),
   - $\rho_b(r)$ is the baryonic mass density at radius $r$,
   - $\nabla^2$ is the Laplacian operator.

3. **Laplacian of Log Density**:
   In spherical coordinates (assuming spherical symmetry for simplicity):
   $$\nabla^2 \log \rho_b(r) = \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial}{\partial r} \log \rho_b(r) \right) = \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{1}{\rho_b(r)} \frac{\partial \rho_b(r)}{\partial r} \right)$$

#### Steps for Computation

1. **Model the Baryonic Density Profile**:
   For a given galaxy, obtain the baryonic mass distribution from observations (e.g., from the SPARC database). Typically, this involves:
   - An exponential disk profile: $\Sigma_d(R) = \Sigma_0 e^{-R / R_d}$ where $R$ is the cylindrical radius, $\Sigma_0$ is the central surface density, and $R_d$ is the scale radius.
   - A bulge profile (if present): e.g., a Hernquist profile $\rho_b(r) = \frac{M_b}{2\pi} \frac{r_b}{r} \frac{1}{(r + r_b)^3}$ where $r_b$ is the scale radius.
   - A gas profile: often modeled as an exponential disk or from HI measurements.
   - Convert these to a spherical density profile $\rho_b(r)$ for simplicity, or use cylindrical coordinates for accuracy.

2. **Compute $\nabla^2 \log \rho_b(r)$**:
   For the spherical case, calculate:
   $$A(r) = \frac{1}{\rho_b(r)} \frac{\partial \rho_b(r)}{\partial r}$$
   $$B(r) = r^2 A(r)$$
   $$C(r) = \frac{1}{r^2} \frac{\partial B(r)}{\partial r}$$
   Thus, $\nabla^2 \log \rho_b(r) = C(r)$.

3. **Compute the Radial Derivative**:
   $$D(r) = \frac{\partial}{\partial r} C(r)$$

4. **Compute Information Acceleration**:
   $$a_{\text{info}}(r) = K \, \log\left( \frac{M_b}{m_p} \right) \, D(r)$$
   where $M_b$ is the total baryonic mass of the galaxy.

5. **Compute Modified Circular Velocity**:
   $$v_c(r) = \sqrt{ \frac{G M_b(r)}{r} + r \, a_{\text{info}}(r) }$$
   where $M_b(r)$ is the cumulative baryonic mass within $r$.

#### Fitting to Data

1. **Data Acquisition**:
   Obtain the observed rotation curve $v_c^{\text{obs}}(r)$ for a galaxy (e.g., from SPARC).

2. **Parameter Fitting**:
   Use a least-squares fitting algorithm (e.g., Levenberg-Marquardt) to determine the best-fit value of the universal constant $K$ that minimizes:
   $$\sum_i \left[ v_c^{\text{obs}}(r_i) - v_c^{\text{predicted}}(r_i, K) \right]^2$$
   The mass-to-light ratios for stellar components should be held within reasonable bounds (e.g., from stellar population synthesis). No free parameters for dark matter are used.

3. **Test the Scaling Relation**:
   Repeat for a large sample of galaxies. The theory predicts that the term $\log(M_b / m_p)$ should capture the variation across galaxies, and a single value of $K$ should provide good fits for all galaxies. This should naturally explain the Tully-Fisher relation (between $M_b$ and $v_c$) and the Radial Acceleration Relation (RAR).

#### Units and Constants

- $K$ has units of $\text{m}^4 / \text{s}^2$.
- $m_p = 1.67 \times 10^{-27} \, \text{kg}$.
- $G = 6.67 \times 10^{-11} \, \text{m}^3 / \text{kg} / \text{s}^2$.
- Ensure consistent units (e.g., masses in kg, distances in m).

#### Example Calculation for a Simple Profile

Assume an exponential disk with spherical approximation for illustration:
- Density profile: $\rho_b(r) = \rho_0 e^{-r / R_d}$ where $\rho_0$ is central density.
- Then:
  $$A(r) = \frac{1}{\rho_b} \frac{\partial \rho_b}{\partial r} = -\frac{1}{R_d}$$
  $$B(r) = r^2 \left( -\frac{1}{R_d} \right) = -\frac{r^2}{R_d}$$
  $$C(r) = \frac{1}{r^2} \frac{\partial B}{\partial r} = \frac{1}{r^2} \left( -\frac{2r}{R_d} \right) = -\frac{2}{r R_d}$$
  $$D(r) = \frac{\partial C}{\partial r} = \frac{\partial}{\partial r} \left( -\frac{2}{r R_d} \right) = \frac{2}{r^2 R_d}$$
- Thus:
  $$a_{\text{info}}(r) = K \, \log\left( \frac{M_b}{m_p} \right) \, \frac{2}{r^2 R_d}$$
- This shows that the information acceleration decreases as $1/r^2$, similar to gravity, but with a strength that depends on the scale length and total mass.

#### Implementation Note

For accurate results, use realistic density profiles (e.g., from photometric data) and compute in cylindrical coordinates if necessary. The Laplacian and derivatives can be computed numerically from data points using finite differences or spline interpolation.

This formulation provides a direct way to test the ToAE by fitting galactic rotation curves without dark matter. The code from the 'ToAE - appendix fractalof derivation' can be extended to perform these calculations numerically.

### References

R. Andrade, P. (2025). Theory of Absolutely Everything - A blueprint to renew human knowledge (19SEP2025). Zenodo. [https://doi.org/10.5281/zenodo.17162302]

R. Andrade, P. (2025). ToAEx-0: Experimental Framework for the Theory of Absolutely Everything (20SEP2025). Zenodo. [https://doi.org/10.5281/zenodo.17166248]

---

This document was produced and refined with the help of artificial intelligence.

This document and its listed documents can be accessed at [https://github.com/pedrora/Theory-of-Absolutely-Everything].

All documents of this theory are released under the _Creative Commons Zero v1.0 Universal_ license and are public domain.
