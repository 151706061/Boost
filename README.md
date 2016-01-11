MIRTK ThirdParty/Boost
======================

This Git submodule repository contains the Boost header files required to build
the MIRTK Numerics, PointSet, and Transformation modules. The respective files
were extracted from the Boost 1.60.0 source distribution package using
[BCP](file:///Users/as12312/Downloads/boost_1_60_0/tools/bcp/doc/html/index.html):

```bash
bcp boost/random.hpp               ThirdParty/Boost
bcp boost/cstdint.hpp              ThirdParty/Boost
bcp boost/config/no_tr1/cmath.hpp  ThirdParty/Boost
bcp boost/math/tools/tuple.hpp     ThirdParty/Boost
bcp boost/numeric/ublas/lu.hpp     ThirdParty/Boost
bcp boost/numeric/ublas/matrix.hpp ThirdParty/Boost
bcp boost/numeric/ublas/vector.hpp ThirdParty/Boost
```

These files can be used instead of an available system Boost installation
after initializing the corresponding MIRTK Git submodule. When the
submodule is not initialized, a separate Boost installation is required.

```bash
cd $MIRTK_SOURCE_DIR
git submodule update --init -- ThirdParty/Boost
```

License
-------

The files in the MIRTK ThirdParty/Boost repository are distributed under the
terms of the Boost Software License Version 1.0.
See accompanying [LICENSE](/LICENSE_1_0.txt) for further information.
