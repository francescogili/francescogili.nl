---
date: "2025-02-20T00:00:00Z"
external_link: ""
image: 
  caption: 
  focal_point: Smart
#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
#slides: example
summary: We propose a new Bayesian nonparametric approach to Wicksell’s problem by placing a Dirichlet Process prior on the observables’ distribution. This simplifies computation via conjugacy and enables asymptotically efficient estimation through projection onto the space of square-integrable, increasing functions. The resulting Isotonized Inverse Posterior (IIP) satisfies a Bernstein–von Mises theorem with minimax variance, adapting to the true cdf’s Hölder continuity without requiring smoothness estimation. 
tags:
- Bayesian inverse problems
- Shape Constraint Inference
title: Bernstein-von Mises phenomenon via Isotonized posterior in Wicksell's problem
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---
We propose a novel Bayesian approach for nonparametric estimation in Wicksell's problem. We deviate from the classical Bayesian nonparametric approach, which would place a Dirichlet Process (DP) prior on the distribution function of the unobservables, by directly placing a DP prior on the distribution function of the observables. Our method offers computational simplicity due to the conjugacy of the posterior and allows for asymptotically efficient estimation by projecting the posterior onto the subspace of square integrable increasing, right-continuous functions. Indeed, the resulting Isotonized Inverse Posterior (IIP) satisfies a Bernstein-von Mises (BvM) phenomenon with minimax asymptotic variance, that depends on the degree of Hölder continuity of the true cdf at the estimation point. Since the IIP gives automatic uncertainty quantification, it eliminates the need to estimate the smoothness of the underlying cdf and other any other parameter. Our results provide the first semiparametric Bernstein–von Mises theorem for projection-based posteriors with a DP prior in inverse problems.

Thus, this approach has three advantages:

1. **Computational speed**: The Dirichlet posterior is explicit, and its projection can be effectively computed using the Pool-Adjacent-Violators Algorithm (PAVA).  

2. **Efficiency and adaptation**: The IIP achieves the asymptotic variance of the efficient estimators introduced in Gili, Jongbloed and van der Vaart (2024), and it is adaptive to the level of local smoothness of the underlying cdf.  

3. **Uncertainty quantification**: The Bayesian framework inherently provides uncertainty quantification without the need to estimate any parameter. We also showed that this is asymptotically correct in the frequentist sense.  

**NEWS: the last version of the paper has been accepted for publication in The Annals of Statistics.** link to last version: https://arxiv.org/pdf/2502.15352
