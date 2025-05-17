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

The object of this research is the stochastic optimization of a smooth, non-convex function. Traditional optimization often assumes $L$-smoothness (Lipschitz continuity of the gradient), but this may appear to be restrictive for real-world deep learning models like Transformers. Instead, we adopt the $(L_0, L_1)$-smoothness condition allowing for a broader class of functions encountered in practice. 

Contributions
========
In this paper we:

     Investigated sign-based methods for communication-efficient distributed optimization under the assumptions above.
     Developed high-probability convergence guarantees accounting for generalized conditions.

The experimental goals are to validate convergence under $(L_0, L_1)$-smoothness and heavy-tailed noise. The setup includes real-world datasets datasets satisfying $(L_0, L_1)$-smoothness with synthetic heavy-tailed noise and convex logistic regression models. The workflow compares sign-based methods against traditional methods, measuring convergence rates and including different accuracy scorings.


Presentations at conferences on the topic of research
===============================
The paper is the part of the larger collective research work. The findings are submitted to NIPS_2025 conference.


Software modules developed as part of the study
======================================================
1. A python package *mylib* with all implementation `will be here <https://github.com/intsystems/ProjectTemplate/tree/master/src>`_.
2. A code with all experiment visualisation `is here <https://github.com/intsystems/Sign-for-L0L1-smooth-opt/blob/master/code/main.ipynb>`_.
