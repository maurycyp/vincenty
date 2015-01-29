# Vincenty
Calculate the geographical distance (in kilometers or miles) between 2 points
with extreme accuracy.

## Example: distance between Boston and New York City
```python
>>> from vincenty import vincenty
>>> boston = (42.3541165, -71.0693514)
>>> newyork = (40.7791472, -73.9680804)
>>> vincenty(boston, newyork)
298.396057
>>> vincenty(boston, newyork, miles=True)
185.414657
```

## Installation
```bash
$ pip install vincenty
```

## See also
* http://en.wikipedia.org/wiki/Vincenty%27s_formulae
* http://en.wikipedia.org/wiki/World_Geodetic_System
