Power
#####

Single Phase Power
******************
.. math:: P = U \cdot I

Three Phase Power
*****************
Power Factor (PF) needs to be accounted for:

PF = 1:

.. math:: P = U \cdot I \cdot \sqrt{3}

PF less than 1:

.. math:: P = U \cdot I \cdot \sqrt{3} \cdot PF

Another approach is to find the phase voltage (using the line to line voltage), and then finding the power with 3 times the phase voltage (assuming PF = 1):

.. math::
   :nowrap:

   \begin{align*}
   U_{phase} &= \frac{U_{line-line}}{\sqrt{3}}\\
   P &= 3 \cdot U_{phase} \cdot I
   \end{align*}

Calculation Examples
====================
Below are examples of calculating three phase power with 400V line to line voltage and 63A of current (assuming PF = 1):

Example 1
---------
.. math::
   :nowrap:

   \begin{align*}
   U_{phase} &= \frac{U_{line-line}}{\sqrt{3}} = \frac{400V}{\sqrt{3}} \approx 230V\\
   P &= 3 \cdot 230V \cdot 63A = 43647.68W \approx 43.7kW
   \end{align*}

Example 2
---------
.. math::
   :nowrap:

   \begin{align*}
   P &= U \cdot I \cdot \sqrt{3} = 400V \cdot 63A \cdot \sqrt{3} = 43647.68W \approx 43.7kW
   \end{align*}


Norwegian Earthing Arrangements
*******************************

IT Network
==========
.. image:: figures/IT.png
    :align: center

TN Network
==========
.. image:: figures/TN.png
    :align: center