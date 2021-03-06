***
mfr
***

**WARNING: mfr is in a very alpha stage of development. As such, it's API is in constant flux. Expect many breaking changes.**

**mfr** (short for "modular file renderer") is a Python package for rendering files to HTML.

.. code-block:: python

    import mfr
    import mfr_image

    # Enable the mfr_image module
    mfr.register_filehandler(mfr_image.Handler)

    with open('hello.jpg') as filepointer:
       mfr.render(filepointer, alt="Hello world")
       # => '<img src="hello.jpg" alt="Hello world" />'


Requirements
============

- Python >= 2.6 or >= 3.3


Available modules
=================

There are a number of 3rd-party modules available.

- `mfr-code-pygments <https://github.com/CenterForOpenScience/mfr-code-pygments>`_
- `mfr_md <https://github.com/TomBaxter/mfr_md>`_

Make your own, then submit a pull request to add it to this list!


Create your own module
======================

Interested in adding support for a new file format? Check out the CONTRIBUTING.rst docs.


License
=======

Copyright 2014 Center for Open Science

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
