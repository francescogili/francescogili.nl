---
date: "2023-10-27T00:00:00Z"
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
summary: We consider the nonparametric estimation in the so-called Wicksell's problem and we show that the isotonized version of the plug-in estimator is asymptotically efficient. The asymptotic variance will depend on the local smoothness at the estimation point and at zero of the unknown distribution function F of the ball squared radii. This solves in an adaptive way the nonparametric estimation problem.
tags:
- Shape Constraint Inference
title: Efficient Isotonic Estimation in Wicksell Problem
url_code: ""
url_pdf: https://arxiv.org/pdf/2310.05463.pdf
url_slides: ""
url_video: ""
---

<script
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
  type="text/javascript">
</script>

<script type="text/javascript"
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-AMS_CHTML">
</script>

<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
    tex2jax: {
      inlineMath: [['$','$'], ['\\(','\\)']],
      processEscapes: true},
      jax: ["input/TeX","input/MathML","input/AsciiMath","output/CommonHTML"],
      extensions: ["tex2jax.js","mml2jax.js","asciimath2jax.js","MathMenu.js","MathZoom.js","AssistiveMML.js", "[Contrib]/a11y/accessibility-menu.js"],
      TeX: {
      extensions: ["AMSmath.js","AMSsymbols.js","noErrors.js","noUndefined.js"],
      equationNumbers: {
      autoNumber: "AMS"
      }
    }
  });
</script>

<div style="text-align: justify">

In this paper we consider nonparametric estimation in the classical Wicksell corpuscle problem: consider an opaque medium that contains randomly positioned 3D spherical particles, that cannot be observed directly. Taking a planar section of the medium, we obtain a sample of observed 2D section profile areas of the intersected particles. The distribution function $F$ of interest is the underlying distribution of the 3D particle squared radii. We take as a starting point the work done in the paper "Isotonic Estimation and Rates of Convergence in Wicksell's problem." by G. Jongbloed and P. Groeneboom, where they introduce the isotonized version of the plug-in estimator, called isotonic estimator, and they analyze it when the underlying $F$ is differentiable at the estimation point $x$. We generalize their setting as we do not require $F$ to be differentiable at $x$ and we allow it to have different degrees of smoothness at that point. 


The main results of this paper are as follows. First, we prove that the isotonic estimator is point-wise asymptotically normal with asymptotic variance that depends on the local degree of smoothness of the underlying distribution function $F$ at $x$. This dependence is expressed through a parameter $\gamma > 1/2$ which can be interpreted as the degree of Hölder smoothness at $x$ of $F$. In this case, the rate of convergence is the usual $(\log{n})^{-1/2} \sqrt{n}$ and the isotonic estimator attains such asymptotic variance in a completely adaptive way, which means without needing knowledge about the true $\gamma$. For $\gamma = 1$, we retrieve the result of Jongbloed and Groeneboom. For the case corresponding to $\gamma = \infty$, i.e. the case $F$ is constant in a neighborhood of the estimation point $x$, we prove a further adaptiveness result as the isotonic estimator attains the $\sqrt{n}$-rate of convergence. In this case, the limiting distribution is not normal. Both these results are novel in their nature and illustrate the adaptiveness of the isotonic estimator.


Concerning the efficiency, we show in the $(\log{n})^{-1/2} \sqrt{n}$ case that the isotonic estimator is also locally asymptotically efficient. We do this by proving a classical lower bound for the minimax risk for any estimator sequence, which also holds under local smoothness conditions of $F$. This shows, whenever all conditions are satisfied, that the previously attained $\gamma$-dependent variance is optimal in the asymptotic minimax sense, and thus the isotonic estimator is asymptotically efficient.

</div>