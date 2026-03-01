---
date: "2026-02-20T00:00:00Z"
external_link: ""
image: 
  caption: 'Initial and deconvolved images of fixed cells. Blue is a nuclear localization signal, green indicates microtubules and red actin filaments. Image from the [Biology Imaging Core at Washington University in Saint Louis](https://www.teledynevisionsolutions.com/learn/learning-center/scientific-imaging/image-restoration-through-deconvolution/).'
  focal_point: Smart
#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
#slides: example
summary: A novel nonparametric Bayesian approach for uncertainty quantification in the deconvolution model Z = X + Y, where the goal is to estimate the distribution of X from noisy observations. By placing a Dirichlet Process prior on the observed data and isotonizing posterior draws via the Greatest Convex Majorant, the Isotonic Inverse Posterior yields computationally fast credible sets with asymptotically correct frequentist coverage, without requiring estimation of any nuisance parameters.
tags:
- Bayesian inverse problems
- Deconvolution
- Uncertainty Quantification
title: Semiparametric Uncertainty Quantification via Isotonized Posterior for Deconvolutions
url_code: ""
url_pdf: "https://arxiv.org/pdf/2602.18210"
url_slides: ""
url_video: ""
---

In many statistical applications, observed data Z_i arises from the sum of two independent components: a variable of interest X_i and another variable Y_i whose distribution is assumed known. This setup applies to many areas of research. For example, X_i might represent a true underlying quantity we aim to measure in an experiment, while Y_i captures additive random measurement error. In epidemiology, X_i could correspond to the actual time of infection and Y_i to the incubation period, as in back-calculation methods used in HIV/AIDS research. The statistical properties of Y_i vary significantly by context: measurement errors are often modeled with symmetric distributions such as the normal, while durations are typically modeled with skewed non-negative distributions such as the Gamma or Weibull.

This method of separating X_i from Y_i is called **deconvolution**, and it arises in many other fields. In image processing, a blurry image Z can be thought of as the true sharp image X convolved with a blur effect Y caused by the camera or optics. In astronomical spectroscopy, the observed spectrum Z is the object's true spectrum X spread by the telescope's point spread function Y. In seismology, recorded seismic waves Z are a combination of the Earth's subsurface structure X and the emitted seismic signal Y; deconvolution is a fundamental step to recover clearer images of the subsurface.

In the domain of nonparametric inference, frequentist methods for deconvolution often yield estimators whose limiting distributions depend on unknown nuisance parameters — such as the density f_0(x) and its derivative — making direct uncertainty quantification difficult in practice. Bayesian nonparametric procedures offer a promising alternative: by leveraging projection-posterior ideas, the resulting credible intervals can achieve asymptotic frequentist coverage that is free of these nuisance parameters.

This paper introduces a novel approach where a **Dirichlet Process prior** is placed directly on the distribution of the observed data Z, yielding a simple, conjugate posterior. To ensure the resulting estimates for F_0 are valid CDFs, we isotonize posterior draws by taking the **Greatest Convex Majorant** of the primitive of each draw, defining what we term the **Isotonic Inverse Posterior**. After a straightforward recalibration based on the Bayes Chernoff distribution, the credible sets achieve asymptotically correct frequentist coverage.

This approach has two key advantages:

1. **Computational speed**: The Dirichlet posterior is explicit and its projection can be effectively computed using the Pool-Adjacent-Violators Algorithm (PAVA).

2. **Uncertainty quantification**: The Bayesian framework inherently provides uncertainty quantification without the need to estimate nuisance parameters, and this is shown to be asymptotically correct in the frequentist sense after appropriate calibration.

The practical effectiveness and robustness of the method are demonstrated through a simulation study with various noise distributions for Y.

**Preprint available on arXiv:** https://arxiv.org/abs/2602.18210

---
*Image: Initial and deconvolved images of fixed cells. Blue is a nuclear localization signal, green indicates microtubules and red actin filaments. Taken from the Biology Imaging Core website at Washington University in Saint Louis. Source: [Teledyne Vision Solutions](https://www.teledynevisionsolutions.com/learn/learning-center/scientific-imaging/image-restoration-through-deconvolution/).*
