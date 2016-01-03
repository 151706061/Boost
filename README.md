MIRTK ThirdParty/Boost
======================

This Git submodule repository contains the Boost header files required to build
the MIRTK Numerics, PointSet, and Transformation modules. The respective files
were extracted from the Boost 1.60.0 source distribution package using the
[BCP](file:///Users/as12312/Downloads/boost_1_60_0/tools/bcp/doc/html/index.html) tool:

```bash
bcp boost/random.hpp               MIRTK/Modules/ThirdParty/Boost
bcp boost/cstdint.hpp              MIRTK/Modules/ThirdParty/Boost
bcp boost/config/no_tr1/cmath.hpp  MIRTK/Modules/ThirdParty/Boost
bcp boost/math/tools/tuple.hpp     MIRTK/Modules/ThirdParty/Boost
bcp boost/numeric/ublas/lu.hpp     MIRTK/Modules/ThirdParty/Boost
bcp boost/numeric/ublas/matrix.hpp MIRTK/Modules/ThirdParty/Boost
bcp boost/numeric/ublas/vector.hpp MIRTK/Modules/ThirdParty/Boost
```

These files can optionally be used instead of an available system Boost installation
after initializing the corresponding MIRTK Git repository submodule. When the
submodule is not initialized, a separate Boost installation is required to build MIRTK.

```bash
cd $MIRTK_SOURCE_DIR
git submodule update --init -- Modules/ThirdParty/Boost
```

License
-------

The files in the MIRTK ThirdParty/Boost repository are distributed under the
terms of the Boost Software License Version 1.0.
See accompanying [LICENSE](/LICENSE_1_0.txt) for further information.
