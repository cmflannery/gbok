.. injectors.rst

Injectors
=========

Injectors are responsible for the distribution, atomization and mixing of propellants into the combustion chamber.
Engine efficiency is closely related to the efficienty of injection.

Design
------

A lot of injector design is based on historical success, however, there are several imporant factors
that must be kept in mind during the design process.

Stability
~~~~~~~~~

Injectors are crucial for combustion stability. Injectors for larger engines commonly have baffels
used to prevent large thermoacoustic waves from arrising in the chamber. Stability is closely coupled
with the choice of elements, thrust per element, element arrangement, and other hydrodynamic flow characteristics.

Achieving a :math:`\delta p` of about :math:`20%` is a common design requirement for reducing one type of
combustion instability: chugging.

Discharge Coefficient
~~~~~~~~~~~~~~~~~~~~~
One important metric in analyzing an injector is the disharge coefficient. It is common to design an injector
to obtain a specific "delta-p" (pressure drop across the injector). This is important to ensure combustion
stability. The discharge coefficient describes the flow restriction of the injector and therefore can
be related to :math:`\delta p` with the following equation.

.. math::
   Q = C_d A \sqrt{2\Delta p/\rho}
