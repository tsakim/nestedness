# Nestedness Calculator for Python
Ths package provides a nestedness calculator for binary matrices, written in 
Python. 

Currently implemented algorithms are:

* [NODF](http://dx.doi.org/10.1111/j.0030-1299.2008.16644.x) (Nestedness based on Overlap and Decreasing Fill) \[AlmeidaNeto2008]

## Author
Mika J. Straka

## This Version
The newest version can be found at [https://github.com/tsakim/nestedness](https://github.com/tsakim/nestedness)

## Usage
Be ``mat`` a two-dimensional binary NumPy array.

* The **NODF** nestedness can be calculated directly without initializing a class instance::
```python
>>> from nestedness_calculator import NestednessCalculator
>>> nodf_score = NestednessCalculator(mat).nodf(mat)
```

When calling ``NestednessCalculator(mat)``, the algorithm checks that the matrix 
is binary and raises an error if it is not. Furthermore, if one or more columns or rows consist only of zeros,
the program aborts.

## Dependencies
The module has been written in *Python 2.7* and uses the following packages:
* [NumPy](http://www.numpy.org/)

## References

\[AlmeidaNeto2008\] [M. Almeida-Neto, P. Guimareas, P. R. Guimaraes, R. D Loyala, W. Ulrich, A consistent metric for nestedness analysis in ecological systems: reconciling concept and measurement, Oikos 117: 1227-1239 (2008)](http://dx.doi.org/10.1111/j.0030-1299.2008.16644.x).

---
Copyright (c) 2017 Mika J. Straka 
