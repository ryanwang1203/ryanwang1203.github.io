---
title: "Surrogate-assisted optimization project"
date: 2025-12-12
---
Wrapped up my MECH 293 final project on surrogate-assisted optimization for a 1D heterogeneous bar.

## Files
- Report: [Mech293FinalProj](/assets/files/Mech293FinalProj.pdf)
- Slides: [Surrogate-Assisted Optimization of a 1D Heterogeneous Bar](/assets/files/Surrogate-Assisted%20Optimization%20of%20a%201D%20Heterogeneous%20Bar.pdf)

## Highlights
- Trained an MLP surrogate to predict **compliance** and **mass** from Young's moduli.
- Test RMSE: **1.27e-2** (compliance), **9.77e-3** (mass).
- Surrogate prescreening reduced FEA calls from **2000 → 50 (~40×)** and found a lower compliance design.

