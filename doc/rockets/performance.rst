.. performance.rst is a list of equations useful for rocket engine design

Rocket Performance
==================

.. note:: The equations presented here are derived for an isentropic rocket engine with constant-pressure
          combustion and steady, one-dimensional flow. For higher fidelity analysis, simulations with
          more realistic assumptions should be performed.
          
The Basic Things
----------------

Thermodynamic Relationships
~~~~~~~~~~~~~~~~~~~~~~~~~~~
Thermodynamic relationships have their foundation in gasses equations of state. I highly recommend
going through the derivation to get to these equations. Shapiro's *The Dynamics and Thermodynamics of Compressible Fluid Flow*
has an excellent explanation and derivation.

.. math::
   \frac{T_0}{T} = 1 + \frac{\gamma-1}{2}M^2

   \frac{p_0}{p}^{(\gamma-1)/\gamma} = \frac{\rho_0}{\rho}^{\gamma-1} = \frac{T_0}{T}

Thrust
~~~~~~

The equation for thrust can be derived from the conservation of momentum by taking a control volume
around the rocket. The result is a function of exhaust velocity (:math:`u_e`), mass flow rate (:math:`\dot{m}`),
exit area (:math:`A_e`), exit pressure (math:`p_e`), and ambient pressure (:math:`p_a`).

.. math::
   T = \dot{m}u_e + (p_e - p_a)*A_e


Specific Impulse
~~~~~~~~~~~~~~~~

A metric that describes the efficiency of the engine. Units of :math:`s`.

.. math::
   I_{sp} = \frac{T}{\dot{m}g_0}

Exhaust Velocity
~~~~~~~~~~~~~~~~

.. math::
   u_e = \sqrt{2 c_p T_{02}\Big[1 - \Big(\frac{p_e}{p_a}^{(\gamma-1)/\gamma}\Big)\Big]}


Propellant Mass Flow Rate
~~~~~~~~~~~~~~~~~~~~~~~~~

.. math::
   \dot{m} = \frac{A^* p_{02}}{\sqrt{R T_{02}}}\sqrt{\gamma \Big(\frac{2}{\gamma + 1}\Big)^{(\gamma+1)/(\gamma-1)}}

Area Ratio
~~~~~~~~~~

.. math::
   \frac{A}{A^*} = \frac{1}{M_e}\Big[\frac{2}{\gamma + 1}\Big(1 + \frac{\gamma - 1}{2}M_e^2\Big)\Big]^{\gamma/(\gamma-1)}

Characteristic Velocity and Thrust Coefficient
-----------------------------------------------

Characteristic Velocity
~~~~~~~~~~~~~~~~~~~~~~~

The characteristic velocity is a function of the combustion chamber properties. As stated below, it
is a function of ratio of specific heats (:math:`\gamma`), specific gas constant (:math:`R`), and
the chamber stagnation temperature (:math:`T_0`)

.. math::
   c^{*} = f(\gamma R T_0) = \frac{p_0 A}{\dot{m}}

Characteristic velocity can be written in a more verbose form,

.. math::
   c^{*} = \sqrt{\frac{1}{\gamma}\Big(\frac{\gamma+1}{2}\Big)^{(\gamma+1)/(\gamma-1)}R T_0}

Thrust Coefficient
~~~~~~~~~~~~~~~~~~

The thrust coefficient is a performance metric used to describe nozzle.

.. math::
    C_T = \frac{T}{p_0 A}

Another form of the thrust coefficient makes the effect of nozzle performance abundantly clear.

.. math::
    C_T  = \sqrt{\frac{2 \gamma^2}{\gamma-1}\Big(\frac{2}{\gamma+1}\Big)^{(\gamma+1)/(\gamma-1)}\Big[1 - \Big(\frac{p_e}{p_0}\Big)^{(\gamma-1)/\gamma}\Big]} + \frac{p_e - p_a}{p_0} \frac{A_e}{A^*}

Combining :math:`c^*` and :math:`C_T` yields an unsurprising result.

.. math::
    T = \dot{m}c^*C_T