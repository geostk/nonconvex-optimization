Non-convex optimization Toolbox
===============================


This matlab toolbox propose a generic solver for proximal gradient descent in the convex or non-convex case. It is a complete reimplementation of the GIST algorithm proposed in [1] with new regularization terms such as the lp pseudo-norm with p=1/2.

The unmix folder contains code downloaded from the website of [ Jose M. Bioucas Dias](http://www.lx.it.pt/~bioucas/publications.html).

When using this toolbox in your research works please cite the following paper:

D. Tuia, R. Flamary and M. Barlaud, "Non-convex regularization in remote sensing", IEEE transactions Transactions on Geoscience and Remote Sensing, (to appear) 2016.

We provide solvers for solving the following estimation problems:
- Least square (linear regression)
- Linear SVM with quadratic Hinge loss
- Linear logistic regression
- Calibrated Hinge loss

The regularization terms that have been coded include:
- Lasso (l1)
- Ridge (squared l2)
- Log sum penalty (LSP) ([2],prox in [1])
- lp regularization with p=1/2
- Group lasso (l1-l2)
- Minimax concave penalty (MCP)

New regularization terms can be easily implemented as discussed in section 3.

# Installation

All the functions in the toolbox a given in the subfolders u/unmix and /utils.

In order to use the function we recommend to execute the following command

```Matlab
addpath(genpath('.'))
```

if you are working in the root folder of the toolbox or replacing '.' by the location of the folder on your machine.


# Entry points

We recommend to look at the following files to see how to use the toolbox:
* demo_classif.m : contains an example of 4 class linear classification problem and show how to learn different classifiers.
* demo_unmix.m : show an example of linear unmixing with positivity constraint and non-convex regularization.
* visu_classif.m : reproduce the example figure in the paper.

# Solving your own optimization problem

## New regularization terms

## Data fitting term


# Contact

* [Rémi Flamary](mailto:remi.flamary@unice.fr)
* [Devis Tuia](mailto:devis.tuia@geo.uzh.ch)

# References

[1] Gong, P., Zhang, C., Lu, Z., Huang, J., & Ye, J. (2013, June). A General Iterative Shrinkage and Thresholding Algorithm for Non-convex Regularized Optimization Problems. In ICML (2) (pp. 37-45).

[2] Candes, E. J., Wakin, M. B., & Boyd, S. P. (2008). Enhancing sparsity by reweighted ? 1 minimization. Journal of Fourier analysis and applications, 14(5-6), 877-905.

Copyright 2016
