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
\begin{abstract}
In Machine Learning, the non-smoothness of optimization problems, the high cost of communicating gradients between workers, and severely corrupted data during training necessitate generalized optimization approaches. This paper explores the efficacy of sign-based methods~\cite{pmlr-v80-bernstein18a}, which address slow transmission by communicating only the sign of each minibatch stochastic gradient. We investigate these methods within $(L_0, L_1)$-smooth problems~\cite{gorbunov}, which encompass a wider range of problems than the $L$-smoothness assumption. Furthermore, under the assumptions above, we investigate techniques to handle heavy-tailed noise~\cite{Kornilov2025}, defined as noise with bounded $\kappa$-th moment $\kappa \in (1,2]$. This includes the use of SignSGD with Majority Voting in the case of symmetric noise. We then attempt to extend the findings to convex cases using error feedback~\cite{karimireddy}.
\end{abstract}

Research publications
===============================
1. TODO

Presentations at conferences on the topic of research
================================================
1. TODO

Software modules developed as part of the study
======================================================
1. A python package *mylib* with all implementation `will be here <https://github.com/intsystems/ProjectTemplate/tree/master/src>`_.
2. A code with all experiment visualisation ` will be here <https://github.comintsystems/ProjectTemplate/blob/master/code/main.ipynb>`_. Can use `colab <http://colab.research.google.com/github/intsystems/ProjectTemplate/blob/master/code/main.ipynb>`_.
