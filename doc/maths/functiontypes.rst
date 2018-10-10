.. useful function types

Functions
=========

Linear
------

A functionm, :math:`f: \mathbb{R}^n \rightarrow \mathbb{R}`, is **linear** if

.. math::

   f(\alpha x + \beta y) = \alpha f(x) + \beta f(y) \\
   \forall x, y \in \mathbb{R}^n \text{ and }\alpha, \beta \in \mathbb{R}

property: :math:`f` is linear if and only if :math:`f(x) = a^Tx` for some :math:`a`

Affine
------

A function, :math:`f: \mathbb{R}^n \rightarrow \mathbb{R}`, is **affine** if

.. math::

   f(\alpha x + (1-\alpha)y) = \alpha f(x) + (1-\alpha)f(y) \\
   \forall x, y \in \mathbb{R}^n \text{ and }\alpha \in \mathbb{R}

property: :math:`f` is linear if and only if :math:`f(x) = a^Tx + b` for some :math:`a`, :math:`b`
