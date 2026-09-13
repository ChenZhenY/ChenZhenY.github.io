---
title: "Covariance Steering for Nonlinear Control-affine Systems"
collection: publications
permalink: /publications/2021-CovarianceSteering/
excerpt: 'Hongzhe Yu, **Zhenyang Chen**, Yongxin Chen'
date: 2021-08-21
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2108.09530'
citation: # 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

We consider the covariance steering problem for nonlinear control-affine systems. Our objective is to find an optimal control strategy to steer the state of a system from an initial distribution to a target one whose mean and covariance are given. Due to the nonlinearity, the existing techniques for linear covariance steering problems are not directly applicable. By leveraging the celebrated Girsanov theorem, we formulate the problem into an optimization over the space path distributions. We then adopt a generalized proximal gradient algorithm to solve this optimization, where each update requires solving a linear covariance steering problem. Our algorithm is guaranteed to converge to a local optimal solution with a sublinear rate. In addition, each iteration of the algorithm can be achieved in closed form, and thus the computational complexity of it is insensitive to the resolution of time-discretization. In the examples, our method achieves 1000 times speedup over an existing algorithm.

[Download paper here](https://arxiv.org/abs/2108.09530)
