---
date: "2023-10-27T00:00:00Z"
external_link: 
image:
  caption: 
  focal_point: Smart
summary: We implemented in Python the Isotonic estimator of the paper "Adaptive and Efficient Isotonic Estimation in Wicksell Problem". We provide the used code where the user can try the estimator choosing from a set of hidden distribution functions F of the radii distribution.
tags:
- Shape Constraint Inference
title: Python implementation of Isotonic Estimator in Wicksell Problem
---
The implementation of the library 

```python 
isotonic_estimator_lib 
```
is essentially based on the PAVA algorithm. Before the publication of this Python Package there was no library in Python that contained the PAVA algorithm (it was available only in R-Studio). See [here](https://pypi.org/project/isotonic-estimator-lib/0.0.7/#description) for the official Python Library.

This package implements the isotonic estimator for Wicksell's problem given in the paper [Adaptive and Efficient Isotonic Estimation in Wicksell's Problem](https://arxiv.org/pdf/2310.05463.pdf). 

How to use the package? After installing the package via the usual command line pip install, the user user can import the package using the lines of code:

```python 
from isotonic_estimator_lib import isotonic_estimator
```

then, having a vector of observed samples Z, the user can obtain the isotonic estimator together with its plot by running:

```python 
max_xs = max(Z)
res = isotonic_estimator.estimator(max_xs,Z)
```

where max_xs is needed for plotting purposes only. The resulting estimated cdf F of the hidden radii distribution is now stored into res. The resulting plot should look as follows: 

![](https://github.com/francescogili/plots_isotonic_estimator_lib/blob/main/test.png?raw=true)

We have also designed a test application in tkinter which is included in the package and where the user can visualize the performance of the isotonic estimator. After running the following code:

```python 
from isotonic_estimator_lib import tester_quality
tester_quality.tester()
```

a pop-up window will open asking to input a test hidden cdf F which can be chosen between the following set of distributions: "gamma, chi, betaprime, pareto, lognormal, truncnorm, arcsine, fatiguelife, weibull". The input is case sensitive. If the user gives non acceptable inputs, the tester will automatically produce an error. The suggested number of samples is 200, and it is not recommended to choose a value higher than 1000. The tester will produce some plots that illustrate the performance of the isotonic estimator. The resulting plot should look like this:

![](https://github.com/francescogili/plots_isotonic_estimator_lib/blob/main/gamma.png?raw=true)

![](https://github.com/francescogili/plots_isotonic_estimator_lib/blob/main/lognormal.png?raw=true)

![](https://github.com/francescogili/plots_isotonic_estimator_lib/blob/main/pareto.png?raw=true)

