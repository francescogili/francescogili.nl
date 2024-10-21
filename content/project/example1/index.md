---
date: "2024-10-20T00:00:00Z"
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
summary: Under smoothness conditions, the Isotonic Inverse Estimator (IIE) achieves an asymptotic convergence rate of √n/logn. If F is constant on an interval around x, the rate improves to √n, with the IIE adapting to this without explicit knowledge. However, the IIE is not asymptotically normal or efficient. The paper introduces three projection-type estimators that leverage the constancy of F and proves their asymptotic efficiency and normality. A local minimax lower bound is also established, and simulation results suggest that the IIE performs comparably to the new estimators despite not being asymptotically equivalent.
tags:
- Shape Constraint Inference
title: Efficient estimation under local constraint in Wicksell's problem
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---
We consider nonparametric estimation in Wicksell's problem which has relevant applications in astronomy for estimating the distribution of the positions of the stars in a galaxy given projected stellar positions (cf. Sen, B. and Woodroofe,  F. N.  (2012)) and in material sciences to determine the 3D microstructure of a material, using its 2D cross sections (cf. Cuzzi, J. and Olson, D. (2017) or  Lopez-Sanchez, M. A. and LLana-Fúnez, S. (2016)). In the classical setting, an opaque medium that contains randomly positioned 3D spherical particles, that cannot be observed directly, is considered. Taking a planar section of the medium, we obtain a sample of observed 2D section profile areas of the intersected particles. The distribution function F of interest is the underlying distribution of the 3D particle squared radii. Under smoothness conditions on F in a neighborhood of x, it was shown in Gili, Jongbloed and van der Vaart (2024) that the Isotonic Inverse Estimator (IIE) is asymptotically efficient, achieving a convergence rate of √n/logn. When F is constant over an interval containing x, the optimal convergence rate improves to √n, and the IIE attains this rate adaptively, without requiring explicit knowledge of the local constancy. However, in this scenario, the asymptotic distribution is non-normal. In this paper, we present three informed projection-type estimators of F, which utilize the interval of constancy information, and show that all three are asymptotically normal and equivalent. Additionally, we establish a local asymptotic minimax lower bound in this context, demonstrating the asymptotic efficiency of the informed estimators, and provide a convolution result indicating that the IIE is not efficient. We also derive the asymptotic distribution of the difference between the IIE and the efficient estimators, confirming that the IIE is not asymptotically equivalent to the informed estimators. Lastly, through a simulation study, we show that even if the IIE is not efficient, its performance closely resembles that of its competitors. Our results cover several novel theoretical findings, which prove essentially that the IIE of Gili, Jongbloed and van der Vaart (2024) is not efficient in the classical statistical sense when F is constant over an interval. On the other hand, we provide estimators that are asymptotically normal and efficient, if the interval of constancy is known. 

Therefore this work is of relevance also from the application point of view, in fields like materials science, astronomy and biosciences, because it shows that the isotonic estimator should not be used by practitioners whenever the underlying F is known to be constant on an interval. Whenever this information is not known, this article confirms that the IIE remains the unequivocal choice for practitioners as its performance is very close to that of the informed competitors and in all other situations it is efficient (c.f. Gili, Jongbloed and van der Vaart (2024)).