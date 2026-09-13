---
layout: page
title: DeepCausalMMM
permalink: /deepcausalmmm/
---

## Overview

A Deep Learning framework for Marketing Mix Modeling with causal structure learning. Standard MMM approaches rely on linear regression or Bayesian hierarchical models that assume channel independence and struggle to capture temporal dynamics and non-linear saturation. DeepCausalMMM combines GRU-based temporal modeling with DAG-based causal discovery to recover channel relationships and time-varying effects that those approaches miss.

## Methodology

- **Temporal modeling**: Gated Recurrent Units (GRUs) learn adstock and lag effects over time.
- **Causal structure learning**: a Directed Acyclic Graph, either an upper-triangular mask or NOTEARS continuous optimization, discovers statistical dependencies between channels instead of assuming independence.
- **Response curves**: Hill equation saturation curves model diminishing returns for budget optimization.
- **Robust statistics**: Huber loss and channel-specific regularization for stability against outliers.
- **Multi-region modeling**: shared and region-specific parameters, with DMA-level economic contribution analysis.

## Paper, code, and docs

- **Paper (JOSS)**: [10.21105/joss.09914](https://doi.org/10.21105/joss.09914)
- **Code**: [github.com/adityapt/deepcausalmmm](https://github.com/adityapt/deepcausalmmm)
- **Install (PyPI)**: `pip install deepcausalmmm`
- **Documentation**: [deepcausalmmm.readthedocs.io](https://deepcausalmmm.readthedocs.io/en/latest/)
- **Tutorial**: [Colab quickstart notebook](https://colab.research.google.com/github/adityapt/deepcausalmmm/blob/main/examples/quickstart.ipynb)
- **Software record (Zenodo)**: [10.5281/zenodo.16934842](https://doi.org/10.5281/zenodo.16934842)

## How to cite

```bibtex
@article{PuttaparthiTirumala2026,
  author  = {Puttaparthi Tirumala, Aditya},
  title   = {DeepCausalMMM: A Deep Learning Framework for Marketing Mix Modeling with Causal Structure Learning},
  journal = {Journal of Open Source Software},
  year    = {2026},
  volume  = {11},
  number  = {120},
  pages   = {9914},
  doi     = {10.21105/joss.09914},
  url     = {https://doi.org/10.21105/joss.09914}
}
```

## Independent discussions

**Technical & practitioner coverage**

- Paolo Baldriga, ["From Bayesian MMM to Deep Causal: Why Storyline Matters More"](https://www.linkedin.com/pulse/from-bayesian-mmm-deep-causal-why-storyline-matters-more-baldriga-4e4ff)
- MachineBrief, ["DeepCausalMMM: Unpacking the Marketing Magic with AI"](https://www.machinebrief.com/news/deepcausalmmm-unpacking-the-marketing-magic-with-ai-q79i)
- 360OM Agency, ["The Future of Marketing Budgets in 2026"](https://www.360om.agency/news-insights/the-future-of-marketing-budgets-in-2026-why-fixed-budgets-will-fail-and-how-to-fix-it)
- Lydec, ["Attribution, CRO, and CAC: A Reality Check"](https://lydec.com/blog/attribution-cro-cac-reality-check)
- SEO by the Sea, ["5-Schritte-Leitfaden zur erfolgreichen Marketingmessung"](https://seo-by-the-sea.de/digital-marketing/sea-performance-marketing/5-schritte-leitfaden-zur-erfolgreichen-marketingmessung) (German)
- Tahereh Nabizadeh, ["Marketing Is Entering a New Scientific Era"](https://www.linkedin.com/posts/tahereh-nabizadeh-70630369_marketing-is-entering-a-new-scientific-era-activity-7440600272080420864-0sbW/) (LinkedIn)
- Buzzhive Marketing, ["Marketing Tracking"](https://buzzhivemarketing.com/marketing-tracking/)

**Research & technical discovery**

- [EmergentMind topic page](https://www.emergentmind.com/topics/deepcausalmmm)
- [Literature review, TheMoonlight.io](https://www.themoonlight.io/en/review/deepcausalmmm-a-deep-learning-framework-for-marketing-mix-modeling-with-causal-inference)
- [llms-explorer.com, Marketing Mix Modeling reference guide](https://llms-explorer.com/sources/mdb-context-hub/da-22-marketing-mix-modeling/)
