CPython Patches
===============

This project is an unofficial fork of `CPython <https://github.com/python/cpython>`_ sources used as
staging area to maintain and test CPython patches.

Fixes and improvements to CPython should first be contributed upstream. The
`Python Developer’s Guide <https://docs.python.org/devguide/>`_ is a great
resource to guide you through the process.

That said, there are few scenarios where maintaining CPython patches is relevant:

* When there is a need for a staging area for patches waiting to be integrated
  upstream. Doing so avoid each project to maintain their own set of patches.

* When the proposed patches are specific to a system not officially supported
  (e.g Android, Emscripten, ...).

* When generalizing proposed patches is definitively not feasible given the
  time and resources.

* When patches fix an older version of CPython (e.g. 2.7) so that it can
  be compiled using newer compiler (e.g VS2015).


Available branches
------------------

* `2.7.3-patches <https://github.com/python/cpython/compare/2.7...python-cmake-buildsystem:2.7.3-patches>`_:

  * Fix build with GNU readline >= 6.3. - Apply to 2.7.3 and 2.7.4

* `2.7.5-patches <https://github.com/python/cpython/compare/2.7...python-cmake-buildsystem:2.7.5-patches>`_:

  * Fix build with GNU readline >= 6.3. - Apply to 2.7.5 and 2.7.6

* `2.7.13-patches <https://github.com/python/cpython/compare/2.7...python-cmake-buildsystem:2.7.13-patches>`_:

  * Support for VS2010 and VS2015. - Apply to 2.7.14 and 2.7.15. See `PythonApplyPatches.cmake <https://github.com/python-cmake-buildsystem/python-cmake-buildsystem/blob/master/cmake/PythonApplyPatches.cmake>`_

* `3.5.3-patches <https://github.com/python/cpython/compare/3.5...python-cmake-buildsystem:3.5.3-patches>`_:

  * Rename header files found in ``Modules/_decimal/libmpdec`` directory to avoid conflicts with system headers
    of the same name (``io.h`` and ``memory.h``). This script was originally used to update the sources: https://gist.github.com/jcfr/e166c0f3fd823de2586b1101f9c67947. - Apply to 3.5.x

  * Prevent duplicated ``OverlappedType`` symbols with built-in extension on Windows. - Apply to 3.5.x

  * Export inlined functions to support extension built-in on Windows. - Apply to 3.5.x

* `3.6.2-patches <https://github.com/python/cpython/compare/3.6...python-cmake-buildsystem:3.6.2-patches>`_:

  * Rename header files found in ``Modules/_decimal/libmpdec`` directory to avoid conflicts with system headers
    of the same name (``io.h``). This script was originally used to update the sources: https://gist.github.com/jcfr/e166c0f3fd823de2586b1101f9c67947. - Apply to 3.6.x

  * Prevent duplicated ``OverlappedType`` symbols with built-in extension on Windows. - Apply to 3.6.x

  * Export inlined functions to support extension built-in on Windows. - Apply to 3.6.x


License
-------

All software is licensed under the Apache 2.0 License.
See `LICENSE_Apache_20 <LICENSE_Apache_20>`_ file for details.

Why Apache 2.0 License?
.......................

From the python.org wiki, the answer to the question `What if I want to
contribute my code to the PSF
<https://wiki.python.org/moin/PythonSoftwareFoundationLicenseFaq#What_if_I_want_to_contribute_my_code_to_the_PSF.3F>`_
mentions that if code is going to end up in Python or the standard library,
the PSF will require you to license code under "Academic Free License" or
"Apache License 2.0".

