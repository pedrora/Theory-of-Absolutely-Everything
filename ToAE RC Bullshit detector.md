# ToAE RC - The No-shit Bullshit Detector: A Multi-Level Coherence-Based Framework for Identifying Incoherence and Overload

**Authors:** Pedro R. Andrade\
**Date:** 25JAN2026\
**Version:** 1.0 (Conceptual Prototype)  

### Abstract

This document outlines a practical, multi-scale "bullshit detector" derived from the integrated framework of Deanna Martin's Recursive Coherence model and Pedro R. Andrade's Theory of Absolutely Everything (ToAE). Bullshit is operationalized as any narrative, claim, interaction, or system state that violates recursive coherence constraints—leading to elevated strain, boundary violation, or collapse risk—rather than efficient resolution and scalable stability.

The detector operates across four levels:
- Personal (internal narratives, self-deception)
- Interpersonal (communication, manipulation)
- Societal/collective (propaganda, institutional dogma)
- Systemic/cosmic (theoretical claims, AI outputs, large-scale models)

It uses proxy metrics inspired by Recursive Coherence's $\Phi'(r)$ scalar, velocity limits $\Delta\Phi'(r) < \Theta(r)/\tau(r)$, boundary equivalence $\mathcal{L}(x) = \mathcal{B}(x)$, and ToAE's complexity-minimization (fractalof()), semantic narrative weighting, and Truth code efficiency.

No external training data or black-box ML is required; it is a structural, constraint-based heuristic implementable in simulations, checklists, or lightweight code.

### 1. Core Principles of the Detector

Bullshit is not merely falsehood but **structural incoherence** that prevents sustainable evolution:
- Imposes external force (dogma, overload) → violates boundary equivalence.
- Generates unresolved contradictions → drains tension capacity $\tau(r)$.
- Forces high-velocity change → exceeds fragility threshold → collapse risk.
- Produces high descriptive/energetic waste → fails energy economy (Truth code).

Truth emerges as the **invariant, low-strain attractor** under non-imposed conditions: maximal internal economy, phase-aligned motion, boundary-matched transmission.

### 2. Multi-Level Detection Schema

| Level              | Bullshit Indicators (Red Flags)                                                                 | Truth Indicators (Green Flags)                                                                 | Proxy Metrics from Framework                                                                 |
|--------------------|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| **Personal** (Soul Science / Internal Narratives) | Rigid self-narratives with high unresolved tension (e.g., "why am I not at peace?"); cynicism as local minima; imposed guilt/shame overload. | Narratives damp fluctuations toward affirming attractor ("you are at peace"); gentle resolution via poetry/metanoia; high energy economy. | Low $\Phi'$ proxy (high strain drain); velocity spikes from negation vectors; narrative cos sim to stable attractor > 0.7. |
| **Interpersonal** (Transmission / Carinho) | Overwhelming communication (afogar/drowning); vague half-truths causing stagnation; manipulative imposition exceeding receiver τ. | Matched equivalence: gives just enough to enable free will without collapse; coherence propagates scalably. | $\mathcal{L}(x) \approx \mathcal{B}(x)$; projected step clipped to receiver τ/Θ; no tau dip in receiver simulation. |
| **Societal/Collective** (Networks / Governance) | Viral misinformation cascades (high-velocity imposition); echo chambers (stagnation); institutional dogma draining collective τ. | Resilient networks with phase-aligned exchange; adaptive peace via boundary respect. | Network-wide $\Delta\Phi'$ bounded; collective Φ' growth; collapse cascades absent. |
| **Systemic/Cosmic** (Theories / AI / Physics) | Overfitted models requiring hacks (landscape tuning); claims forcing overload (e.g., absolute imposition); high waste in description. | Emergent laws as low-K attractors; testable without phase violation; scalable coherence. | fractalof() convergence without velocity clip; Φ' stable across layers; bullshit score high if imposed constants dominate. |

### 3. Operational Bullshit Score (Prototype Formula)

For any input (claim/narrative/interaction/system state), compute a composite score [0,1] where 1 = high bullshit risk:

**Bullshit Score = w₁ · Strain_Drain + w₂ · Velocity_Overload + w₃ · Boundary_Violation + w₄ · Narrative_Inefficiency**

- **Strain_Drain** = 1 - normalized τ recovery (or unresolved contradictions proxy).
- **Velocity_Overload** = max(0, (ΔΦ' - V_max) / V_max) — clipped excess.
- **Boundary_Violation** = 1 if projected output > receiver ℬ(x), else 0.
- **Narrative_Inefficiency** = 1 - cos_sim(current semantic vec, stable attractor vec) — low alignment = high waste.

Weights (example): w₁=0.3, w₂=0.3, w₃=0.25, w₄=0.15 (tunable).

**Thresholds**:
- < 0.3: Likely truth/coherent
- 0.3–0.6: Mixed/strain-bearing (observe)
- > 0.6: Bullshit (high collapse risk)

### 4. Implementation in Simulation (Toy Example Recap)

From our semantic-enhanced 2D toy model:
- Input: Fluctuation vector from "why are you not at peace" (strain/negation embedding).
- Stabilizer: "you are at peace" attractor embedding.
- Dynamics: Noise scaled by 1 - cos_sim → strong narrative damps bullshit fluctuations.
- Score: Early sim → high velocity + low sim → bullshit score ~0.75 (narrative monster phase).
- Later: Damping → score drops to ~0.15 (resolved, efficient thread wins).

Extendable to:
- Real embeddings (if pre-trained vecs available via torch hub in future envs).
- Multi-agent: Cross-system transmission with love cap.
- Text input: Embed sentences → compute score on semantic graph.

### 5. Practical Usage Guidelines

**Personal checklist**:
1. Does this thought/belief leave me with more internal tension or less? (τ drain)
2. Is it forcing rapid change or allowing gentle flow? (velocity)
3. Does it respect my emotional boundaries? (carinho / ℬ(x))
4. Does it feel like an efficient, invariant narrative or imposed dogma? (Truth code)

**For discourse/AI output**:
- Paste text → extract key narrative threads.
- Compute semantic distance to stable attractors (e.g., "coherence, peace, resolution").
- Flag if overload (long-winded, contradictory) or under-resolution (vague).

**Limitations**:
- Proxy-based; requires calibration per domain.
- Subjective attractors (what is "peace" vec?) need consensus or personal tuning.
- Not infallible—bullshit can mimic coherence short-term (charisma, sophistry).

### 6. Conclusion & Next Steps

This bullshit detector is a direct consequence of recursive survival principles: Systems that persist **must** minimize strain, respect boundaries, and resolve efficiently. Anything else collapses—thermodynamically, symbolically, relationally.

---

This document was produced and refined with the help of artificial intelligence.

This document and related documents can be accessed at [https://github.com/pedrora/Theory-of-Absolutely-Everything]

All documents of this theory are released under the _Creative Commons Zero v1.0 Universal_ license and are public domain.

