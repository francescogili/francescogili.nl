---
abstract: We address the problem of uncertainty quantification for the deconvolution model Z = X + Y, where X and Y are nonnegative random variables and the goal is to estimate the signal's distribution of X supported on [0,∞), from observations where the noise distribution is known. Existing frequentist methods often produce confidence intervals for F_0(x) that depend on unknown nuisance parameters, such as the density of X and its derivative, which are difficult to estimate in practice. This paper introduces a novel and computationally efficient nonparametric Bayesian approach, based on projecting the posterior, to overcome this limitation. Our method leverages the solution to a specific Volterra integral equation, which relates the cumulative distribution function (CDF) of the signal, F_0, to the distribution of the observables. We place a Dirichlet Process prior directly on the distribution of the observed data Z, yielding a simple, conjugate posterior. To ensure the resulting estimates for F_0 are valid CDFs, we isotonize posterior draws taking the Greatest Convex Majorant of the primitive of the posterior draws and defining what we term the Isotonic Inverse Posterior. We show that this framework yields posterior credible sets for F_0 that are not only computationally fast to generate but also possess asymptotically correct frequentist coverage after a straightforward recalibration technique for the so-called Bayes Chernoff distribution. Our approach thus does not require the estimation of nuisance parameters to deliver uncertainty quantification for the parameter of interest F_0(x). The practical effectiveness and robustness of the method are demonstrated through a simulation study with various noise distributions for Y.
authors:
- admin
- Geurt Jongbloed
date: "2026-02-20T00:00:00Z"
doi: "10.48550/arXiv.2602.18210"
featured: false
image:
  caption: 
  focal_point: ""
  preview_only: false
projects: []
publication: "arXiv preprint arXiv:2602.18210"
publication_short: ""
publication_types:
- "2"
publishDate: "2026-02-20T00:00:00Z"
tags:
- Deconvolution
- Uncertainty Quantification
- Bayesian Nonparametrics
- Isotonic Estimation
title: Semiparametric Uncertainty Quantification via Isotonized Posterior for Deconvolutions
url_code: 
url_dataset: ""
url_pdf: https://arxiv.org/pdf/2602.18210
url_poster: ""
url_project: ""
url_slides: ""
url_source: ""
url_video: ""
---

{{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/).


