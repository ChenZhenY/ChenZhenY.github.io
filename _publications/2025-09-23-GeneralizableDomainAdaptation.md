---
title: "Generalizable Domain Adaptation for Sim-and-Real Policy Co-Training"
collection: publications
permalink: https://ot-sim2real.github.io/
excerpt: 'Shuo Cheng, Liqian Ma, **Zhenyang Chen**, Ajay Mandlekar, Caelan Garrett, Danfei Xu'
date: 2025-09-23
venue: 'Advances in Neural Information Processing Systems (NeurIPS) 2025'
paperurl: 'https://arxiv.org/abs/2509.18631'
citation: # 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

Behavior cloning has shown promise for robot manipulation, but real-world demonstrations are costly to acquire at scale. While simulated data offers a scalable alternative, particularly with advances in automated demonstration generation, transferring policies to the real world is hampered by various simulation and real domain gaps. In this work, we propose a unified sim-and-real co-training framework for learning generalizable manipulation policies that primarily leverages simulation and only requires a few real-world demonstrations. Central to our approach is learning a domain-invariant, task-relevant feature space. Our key insight is that aligning the joint distributions of observations and their corresponding actions across domains provides a richer signal than aligning observations (marginals) alone. We achieve this by embedding an Optimal Transport (OT)-inspired loss within the co-training framework, and extend this to an Unbalanced OT framework to handle the imbalance between abundant simulation data and limited real-world examples. We validate our method on challenging manipulation tasks, showing it can leverage abundant simulation data to achieve up to a 30% improvement in the real-world success rate and even generalize to scenarios seen only in simulation.

[Website](https://ot-sim2real.github.io/)
