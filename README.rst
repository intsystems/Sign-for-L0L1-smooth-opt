|test| |codecov| |docs|

.. |test| image:: https://github.com/intsystems/ProjectTemplate/workflows/test/badge.svg
    :target: https://github.com/intsystems/ProjectTemplate/tree/master
    :alt: Test status
    
.. |codecov| image:: https://img.shields.io/codecov/c/github/intsystems/ProjectTemplate/master
    :target: https://app.codecov.io/gh/intsystems/ProjectTemplate
    :alt: Test coverage
    
.. |docs| image:: https://github.com/intsystems/ProjectTemplate/workflows/docs/badge.svg
    :target: https://intsystems.github.io/ProjectTemplate/
    :alt: Docs status


.. class:: center

    :Название исследуемой задачи: Sign operator for $(L_0, L_1)$ smooth opitization
    :Тип научной работы: M1P
    :Автор: Иконников Марк Игоревич
    :Научный руководитель: Beznosikov Aleksandr Nikolaevich, PhD
    :Научный консультант(при наличии): MS student Korniliv Nikita Maksimovich

Abstract
========

In Machine Learning, the non-smoothness of optimization problems, the high cost of communicating gradients between workers, and severely corrupted data during training necessitate generalized optimization approaches. This paper explores the efficacy of sign-based methods, which address slow transmission by communicating only the sign of each minibatch stochastic gradient. We investigate these methods within $(L_0, L_1)$-smooth problems, which encompass a wider range of problems than the $L$-smoothness assumption. Furthermore, under the assumptions above, we investigate techniques to handle heavy-tailed noise, defined as noise with bounded $\kappa$-th moment $\kappa \in (1,2]$. This includes the use of SignSGD with Majority Voting in the case of symmetric noise. We then attempt to extend the findings to convex cases using error feedback.


Problem Statement
========

A function $f : \mathbb{R}^d \to \mathbb{R}$ is said to be \textit{$(L_0, L_1)$-smooth} if
\[
\|\nabla f(x) - \nabla f(y)\| \leq (L_0 + L_1 \sup_{u \in [x,y]} \|\nabla f(u)\|) \|x - y\|.
\]
This generalizes classical $L$-smoothness and captures many practical functions that appear in deep learning.

The noise model assumes that the stochastic gradients $\nabla f(x, \xi)$ have bounded $\kappa$-th moment:
\[
\mathbb{E}_\xi [|\nabla f(x, \xi)_i - \nabla f(x)_i|^\kappa] \leq \sigma_i^\kappa, \quad \text{for all } i \in [d], \quad \kappa \in (1,2].
\]

Presentations at conferences on the topic of research
===============================
The paper is the part of the larger collective research work. The findings are projected to be submitted to NIPS_2025 conference.


Software modules developed as part of the study
======================================================
1. A python package *mylib* with all implementation `will be here <https://github.com/intsystems/ProjectTemplate/tree/master/src>`_.
2. A code with all experiment visualisation `is here <https://github.com/intsystems/Sign-for-L0L1-smooth-opt/blob/master/code/main.ipynb>`_.
