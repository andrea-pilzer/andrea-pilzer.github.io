---
layout: post
title: "Log-Sum-Exp paper accepted at NeurIPS 2026!"
date: 2026-11-03 12:00:00 +0100
categories: jekyll update
---

Our [paper on speeding up Log-Sum-Exp](https://arxiv.org/abs/2610.33647) has been accepted at NeurIPS 2026! We introduce faster CPU and GPU kernels for this key operation underlying softmax, with potential benefits for AI models that rely heavily on it.

- **CPU:** Approximate integer arithmetic accelerates the computation, tested on particle filtering.
- **GPU:** Kernel fusion reduces memory traffic and launch overhead, tested on RLHF log-probability computation and probabilistic circuit inference.
