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

* `2.7.13-patches <https://github.com/python/cpython/compare/2.7...python-cmake-buildsystem:2.7.13-patches>`_:

  * Support for VS2010 and VS2015


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

