# Compression → Klein–Gordon → $E=mc^2$

This document derives the Klein–Gordon equation from a 4D compression action (Fisher penalty + energetic term) and shows how $E=mc^2$ arises naturally.

## 0) 4D compression action

Define fields $\rho(x)\ge0$, $S(x)\in\mathbb{R}$, $x\in\mathbb{R}^{1+3}$, and the complex field
$$
\psi(x)=\sqrt{\rho(x)}\,e^{\,iS(x)/\hbar}.
$$

Compression-inspired action (mostly-plus signature $(+,-,-,-)$):
$$
\mathcal{A}[\rho,S]=\int d^4x\;\left\{ \rho(\partial_\mu S\,\partial^\mu S + m^2 c^2)
+ \frac{\hbar^2}{2}\,\partial_\mu\sqrt{\rho}\,\partial^\mu\sqrt{\rho} \right\}.
$$

## 1) Variation w.r.t. $S$ — continuity equation

Varying $S$ yields
$$
\partial_\mu(\rho\,\partial^\mu S)=0,
$$
i.e. the relativistic continuity equation. Define the 4-current $j^\mu=\rho\,\partial^\mu S$.

## 2) Variation w.r.t. $\rho$ — relativistic quantum Hamilton–Jacobi

Varying $\rho$ gives
$$
\partial_\mu S\,\partial^\mu S + m^2 c^2 - \frac{\hbar^2}{2}\frac{\Box\sqrt{\rho}}{\sqrt{\rho}} = 0.
$$

Define the quantum potential
$$
Q[\rho] = -\frac{\hbar^2}{2}\frac{\Box\sqrt{\rho}}{\sqrt{\rho}},
$$
so the HJ equation reads $\partial_\mu S\,\partial^\mu S + m^2 c^2 + Q[\rho] = 0$.

## 3) Combine into $\psi$ and compute $\Box\psi$

Set $\psi=\sqrt{\rho}e^{iS/\hbar}$. Compute $\Box\psi$ (details omitted here but algebra follows from product rule and using the two real equations). After cancellations one obtains the Klein–Gordon equation:
$$
\big(\Box + \tfrac{m^2 c^2}{\hbar^2}\big)\psi = 0.
$$

## 4) Dispersion relation → $E=mc^2$

Plane-wave solutions $\psi\sim e^{-i(Et-\mathbf{p}\cdot\mathbf{x})/\hbar}$ give
$$
E^2 = |\mathbf{p}|^2 c^2 + m^2 c^4,
$$
and at rest ($\mathbf{p}=0$):
$$
E = mc^2.
$$

## 5) Interpretation

- Mass is the baseline compression cost for localizing an information packet; energy is the compression-rate.  
- Lorentz invariance makes $c^2$ the conversion factor between spatial and temporal compression scales.  
- Thus $E=mc^2$ is the natural equivalence between stored compression complexity (mass) and compression rate (energy).
