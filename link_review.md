# Link Review

- 3 key articles for the research
- additional papers for specific methods and/or proofs

| Topic | Title | Year | Authors | Paper | Summary |
| :--- | :--- | ---: | :--- | :--- | :--- | :--- |
| Key article 1 | Sign Operator for Coping with Heavy-Tailed Noise | 2025 | Kornilov et al. | [arXiv](https://arxiv.org/abs/2502.07923) | Proofs for heavy-tailed noise |
| Key article 2 | signSGD: Compressed Optimisation for Non-Convex Problems | 2018 | J. Bernstein et al. | [PMLR](https://proceedings.mlr.press/v80/bernstein18a.html) | 3 Sign-based methods |
| Key article 3 | Methods for Convex (L0,L1)-Smooth Optimization: Clipping, Acceleration, and Adaptivity | 2024 | Gorbunov et al. | [arXiv](https://arxiv.org/abs/2409.14989) | New convergence guarantees for existing methods |
| Theory |Robustness to Unbounded Smoothness of Generalized SignSGD | 2022 | M. Crawshaw et al. | [Curran Associates](https://proceedings.neurips.cc/paper_files/paper/2022/file/40924475a9bf768bdac3725e67745283-Paper-Conference.pdf) | L_0, L1 Sign SGD with Momentum |
| Advanced theory | EF21: A New, Simpler, Theoretically Better, and Practically Faster Error Feedback | 2021 | Richtárik et al. | [arXiv](https://arxiv.org/abs/2106.05203) | SOTA error feedback algorithm with sound theoretical analysis |
| Advanced theory | A High Probability Analysis of Adaptive SGD with Momentum | 2020 | Li & Orabona | [arXiv](https://arxiv.org/abs/2007.14294) | Important Measure Concentration Lemma and an example of proving high-probability convergence |
| Experimental evidence | Why are Adaptive Methods Good for Attention Models? | 2020 | Zhang et al. | [arXiv](https://arxiv.org/abs/1912.03194) | 1) Empirical and theoretical evidence that a heavy-tailed distribution of the noise in stochastic gradients causes poor performance of SGD. 2) Gradient clipping can deal with that + BERT training.
| Competitors | From Gradient Clipping to Normalization for Heavy Tailed SGD | 2024 | Hübler et al. | [arXiv](https://arxiv.org/abs/2410.13849) | Normalized SGD with heavy tails under heavy-tailed noise and a proof of Batching Lemma |
