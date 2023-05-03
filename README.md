<div>
<img src="img/Princeton_logo.png" width="200" align="left"/>
</div>

<div>
<img src="img/IRIS-HEP_logo.png" width="150" align="right"/>
</div>

# Awkward Just-In-Time (JIT) Compilation: A Developer’s Experience


Awkward Array is a library for performing NumPy-like computations on nested, variable-sized data, enabling array-oriented programming on arbitrary data structures in Python. However, imperative (procedural) solutions can sometimes be easier to write or faster to run. Performant imperative programming requires compilation; JIT-compilation makes it convenient to compile in an interactive Python environment.

Several functions in Awkward Arrays JIT-compile a user’s code into executable machine code. They use several different techniques, but reuse parts of each others’ implementations.

We discuss the techniques used to achieve the Awkward Arrays acceleration with JIT-compilation, focusing on RDataFrame, cppyy, and Numba, particularly Numba on GPUs:

* Conversions of Awkward Arrays to and from RDataFrame
* Standalone cppyy
* Passing Awkward Arrays to and from Python functions compiled by Numba
* Passing Awkward Arrays to Python functions compiled for GPUs by Numba
* Header-only libraries for populating Awkward Arrays from C++ without any Python dependencies

## Authors
Angus Hollands, Ioana Ifrim, Ianna Osborne, Jim Pivarski, Henry Schreiner

Princeton University, Princeton, NJ 08544, USA

## Acknowledgements
<div>
<img src="img/NSF_logo.png" width="60" align="left"/>
</div>

Support for this work was provided by NSF cooperative agreement [OAC-1836650](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1836650) (IRIS-HEP)
