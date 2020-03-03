<img src="https://github.com/Antonio-Cruciani/Nystrom-Low-Rank-Approximation/blob/master/img/nystrom_lowrank.png?v=3&s=200" title="Nystrom Approximation" alt="Nystrom" height=300 width=700>


# Nystrom-Low-Rank-Approximation
Nystrom Low Rank Gram Matrix Approximation in KELP


## Table of Contents 

- [Description](#Description)
- [Nystrom Method](#Nystrom-Method)
- [Kelp](#Kelp)
- [Examples](#Examples)
- [License](#License)

## Description

This library allows you to use Kernel Methods for large-scale learning problems.

## Nystrom-Method

Kernel methods project data points into a high dimensional or infinite-dimensional feature space and find the optimal splitting hyperplane. In the kernel method the data is represented in a Gram Matrix. The main problem of kernel method is its high computational cost associated with kernel matrices. The cost is at least quadratic in the number of training data points, but most kernel methods include computation of matrix inversion or eigenvalue decomposition and the cost becomes cubic in the number of training data Large training sets cause large storage and computational costs. In spite of low rank decomposition methods (Cholesky decomposition) reduce this cost, they continue to require computing the kernel matrix. One of the approaches to deal with this problem is low-rank matrix approximations. The most popular examples of them are Nyström method and the random features.

The Nyström approximation can allow a significant speed-up of the computations. This speed-up is achieved by using instead of the kernel matrix its approximation of a smaller rank.