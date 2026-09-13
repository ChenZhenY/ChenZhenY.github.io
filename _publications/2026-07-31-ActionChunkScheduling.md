---
title: "Action Chunk Scheduling for Batched Robot Policy Serving"
collection: publications
permalink: https://gatech-rl2.github.io/actionchunkscheduling/
excerpt: 'Rohan Bansal, David He, Nadun Ranawaka Arachchige, **Zhenyang Chen**, Soobum Kim, Kexin Rong, Danfei Xu'
date: 2026-07-31
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2608.00337'
citation: # 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

Deploying robot foundation models at scale is the next step towards realizing the potential of general-purpose robots. However, Vision-Language-Action (VLA) and other foundation models are computationally demanding, and on-device compute is constrained by power and space. In this paper, we introduce the problem of serving a robot policy to multiple robots from a remote GPU and formulate it as a scheduling problem. We build Armory, a serving system validated on fleets of both simulated and real robots. Our experiments show that naive scheduling heuristics perform well when all robots are the same, but fall short when robots consume action chunks at different rates, uncovering a mismatch between conventional batching methods and the closed-loop requirements of robot policy execution. To address this, we propose a scheduling algorithm that accounts for this heterogeneity and improves overall system throughput by up to 18% in real-world experiments.

[Website](https://gatech-rl2.github.io/actionchunkscheduling/)
