---
layout: page
title: CausalGeo
permalink: /causalgeo/
---

## Overview

CausalGeo is a Python package for estimand-first geo incrementality: concurrent geo holdouts for bundle lift and calibrated channel responses. It measures the lift of a media bundle, then uses impression paths for a clearly labeled, model-assisted channel split only when the experimental design can separate the channels.

The package is deliberately explicit about what a geo experiment can and cannot identify. A bundled holdout measures a bundled effect; it does not turn each channel in that bundle into a separate experiment.

## What it does

- **Concurrent geo holdouts**: runs several media bundles in the same weeks, each with its own control markets.
- **Bundle-level lift**: estimates lift, percent lift, and incremental cost per dollar with time-based regression by default, plus synthetic control, synthetic difference-in-differences, and clustered two-way fixed effects.
- **Calibrated channel responses**: combines impression history with measured bundle lift while labeling channel results as model-assisted rather than experimental estimates.
- **Identification-aware reporting**: withholds a channel estimate when the design cannot distinguish that channel, rather than reporting false precision.
- **Prior-aware allocation**: can update an external MMM prior with bundle-level experimental evidence while showing how many independent directions the experiment actually tested.

## Availability

- **Code**: [github.com/adityapt/causalgeo](https://github.com/adityapt/causalgeo)
- **Install**: `pip install "causalgeo @ git+https://github.com/adityapt/causalgeo.git@v0.2.4"`
- **License**: MIT
- **Software record**: [10.5281/zenodo.24041239](https://doi.org/10.5281/zenodo.24041239)
- **Manuscript**: submitted to *SoftwareX*

## Citation

The *SoftwareX* manuscript is under review. Until it is published, cite the archived v0.2.4 release: [10.5281/zenodo.24041239](https://doi.org/10.5281/zenodo.24041239).
