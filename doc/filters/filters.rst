.. notes on filtering

Filtering, Smoothing and Predicting
==================================

Overview
--------

Linear Programming is a method by which an optimal, minimum or maximum, outcome is obtained for
mathamatical models formed from linear functions of decision variables subject to constraints.

Typically, a linear program (LP) takes the following form.

.. math::
   
   \text{min }\sum{c^{T}x} \\
   \text{subject to }Ax = b \\
   l \le x \le u

where :math:`\sum{c^{T}x}` is the cost function or objective function, :math:`x_j` is the
optimization variable, and :math:`Ax = b` and :math:`l \le x \le u` are constraints. In such a
problem, :math:`A, b, c, l,` and :math:`u` are assumed to be known parameters of the mathematical
model.

Important Concepts
------------------

Review the following concepts.

.. toctree::
   linear_programming/geometry_of_lp

Solving Linear Programs
-----------------------

LPs can be efficiently solved with the following numerical methods:
   - simplex, dual simplex method
   - interior point methods for LPs with very sparse matricies
   - decomposition, dual decomposition and regularized decomposition approaches for LP’s with 
     special block structures of their coefficient matrices A

Stochastic Linear Programs
--------------------------

In many applications of Linear Programming, exact values are not known for the mathematical model;
rather, expectations are used. As a result, the solution must be computed with different methods in
order to achieve a desired probability distribution, rather than a known solution.