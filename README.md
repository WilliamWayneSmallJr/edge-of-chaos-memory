# Edge-of-Chaos Memory Under Noise

This repository contains empirical experiments comparing **first-order (FO)** and **second-order (SO)** local dynamical systems under stochastic noise, with a focus on **mutual-information retention** and **regime dependence**.

## Summary of Findings

Across elementary cellular automata (ECA), we observe a clear phase boundary:

- **Chaotic regimes (e.g. Rule 30):**  
  Second-order dynamics provide no advantage over first-order dynamics under noise.

- **Critical / structured regimes (e.g. Rule 110):**  
  Second-order dynamics consistently retain more mutual information than first-order dynamics under annealed noise.

- **Linear regimes (e.g. Rule 150):**  
  The advantage of second-order dynamics is strongest.

These results demonstrate that recursive memory benefits are **regime-dependent**, appearing near the *edge of chaos* rather than universally.

## Methodology

- Local dynamics: elementary cellular automata  
- Comparison: first-order vs second-order (two-slice) updates  
- Noise: annealed stochastic bit-flip noise  
- Metric: normalized mutual information I(W₀;Wₜ) / H(W₀)  
- Controls: permutation null baselines and negative-rule tests  
- Implementation: lightweight Python (runs on commodity hardware)

Claims of universality or noise-free reversibility are explicitly rejected by the data.

## Status

This repository serves as a **public experimental record** and prior-art disclosure.
Code, plots, and parameter details are provided for transparency and replication.

## Author

Independent research by William Wayne Small Jr.
