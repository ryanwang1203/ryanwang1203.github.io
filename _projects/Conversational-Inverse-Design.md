---
layout: single
title: "Conversational Inverse Design of Cellular Structures in Implicit Field Space"
date: 2026-01-06
excerpt: "Conversational inverse design framework that lets a user describe the behavior they want in natural language and receive multiple candidate unit-cell geometries represented directly in implicit field space."
one_liner: "Conversational inverse design framework that lets a user describe the behavior they want in natural language and receive multiple candidate unit-cell geometries represented directly in implicit field space."
highlights:
  - "We introduce a large-scale implicit-field dataset of periodic cellular structures generated from analytic families with parameterized transformations. Each sample includes ground-truth metadata that enables controlled studies of periodicity and morphology."
  - "We present a conversational inverse design pipeline that translates natural-language intent into structured targets and constraints, and proposes multiple candidate unit cells via retrieval in implicit field space to reflect the one-to-many nature of the problem."
  - "We define a verification-first evaluation protocol that reports target-matching error, success rate under strict tolerances, diversity among valid solutions, and computational cost, and we benchmark against a strong retrieval baseline with constraint filtering and diversity selection."
---

- **Paper:** [IDETC26](/assets/files/Conversational_IDETC26.pdf)

## Highlights
{% for h in page.highlights %}
- {{ h }}
{% endfor %}
