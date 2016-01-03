Vincenty
========

Calculate the geographical distance (in kilometers or miles) between 2 points
with extreme accuracy.

This library implements Vincenty's solution to the inverse geodetic problem. It
is based on the WGS 84 reference ellipsoid and is accurate to within 1 mm (!) or
better.

This formula is widely used in geographic information systems (GIS) and is much
more accurate than methods for computing the great-circle distance (which assume
a spherical Earth).

Example: distance between Boston and New York City
--------------------------------------------------

.. code:: python

   >>> from vincenty import vincenty
   >>> boston = (42.3541165, -71.0693514)
   >>> newyork = (40.7791472, -73.9680804)
   >>> vincenty(boston, newyork)
   298.396057
   >>> vincenty(boston, newyork, miles=True)
   185.414657


Installation
------------

.. code:: bash

   $ pip install vincenty


References
----------

* https://en.wikipedia.org/wiki/Vincenty's_formulae
* https://en.wikipedia.org/wiki/World_Geodetic_System
