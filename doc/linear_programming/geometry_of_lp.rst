.. geometry of linear programs


Geometry of Linear Programs
===========================

Convex Sets
-----------

A set of points is called a *convex* set if all the points on the straight line segment joining any
two points in the set belong to the set.

.. image:: resources/convex_sets.png
   :width: 500px
   :alt: alternate text
   :align: center

Affine Sets
-----------

Affine sets: allows us to describe a set independently of system of coordinates

.. note::
   line going through the origin defines a Subspace
   i.e. :math:`y = ax`

   line going through through :math:`y(0) = b`, or defined by :math:`y=ax+b` defines an affine set

Affine sets let us define systems independent of the origin.

.. note:: Parallel Subspace
   To every set :math:`C`, we can associate a subspace :math:`V` called a "parallel subspace"

The dimension of a parallel subspace can be defined by the affinely independent vectors of the subspace
!add formal definition!

Every affine set can be expressed as the set of solutions of linear equations.
 
.. rubric:: References

.. [1] Dantzig, G. Bernard, `Linear Programming and Extensions`_. RAND Report. August 1963. Chapter 7.


.. _Linear Programming and Extensions: https://www.rand.org/pubs/reports/R366.html