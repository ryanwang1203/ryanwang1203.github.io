---
title: "Surrogate-Assisted Optimization of a 1D Heterogeneous Bar (MECH 293)"
date: 2025-12-12
one_liner: "FEA ground-truth + neural surrogate to accelerate compliance minimization under mass constraints."
highlights:
  - "Implemented 1D linear FEA as ground truth solver"
  - "Trained a neural network surrogate for compliance and mass prediction"
  - "Used the surrogate in an optimization loop to speed up exploration"
links:
  - label: "Report (PDF)"
    url: "#"
  - label: "Code"
    url: "#"
---

## Problem
Minimize compliance of a 1D heterogeneous bar with spatially varying Young’s modulus under a mass constraint.

## Approach
- Ground truth: linear FEA
- Surrogate: fully-connected network mapping element-wise stiffness → compliance & mass
- Optimization: use surrogate predictions to guide search (with periodic ground-truth checks)

## What to add
Replace the placeholder links with:
- your final report PDF
- your GitHub repo (or a public code excerpt)
