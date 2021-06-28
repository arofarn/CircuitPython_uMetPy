Introduction
============


.. image:: https://readthedocs.org/projects/circuitpython-umetpy/badge/?version=latest
    :target: https://circuitpython-umetpy.readthedocs.io/
    :alt: Documentation Status


.. image:: https://img.shields.io/discord/327254708534116352.svg
    :target: https://adafru.it/discord
    :alt: Discord


.. image:: https://github.com/arofarn/CircuitPython_uMetPy/workflows/Build%20CI/badge.svg
    :target: https://github.com/arofarn/CircuitPython_Org_uMetPy/actions
    :alt: Build Status


.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code Style: Black

Small subset of MetPy python module for CircuitPython.

Come without numpy, pint (units), matplotlib or other "big" library support.

As pint is not supported, the SI units are used.


Original project : `MetPy <https://unidata.github.io/MetPy/latest/index.html>`_

Dependencies
=============
This library depends on:

* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_

Please ensure all dependencies are available on the CircuitPython filesystem.
This is easily achieved by downloading
`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.


Usage Example
=============

.. code-block:: python3

    import umetpy.constants

    print("List of all constants:\n")
    for cst in dir(umetpy.constants):
        if cst[0] != "_":
            print("{:25s} = {:f}".format(cst, eval("{}.{}".format("umetpy.constants", cst))))

Contributing
============

Contributions are welcome! Please read our `Code of Conduct
<https://github.com/arofarn/CircuitPython_Org_uMetPy/blob/HEAD/CODE_OF_CONDUCT.md>`_
before contributing to help this project stay welcoming.

Documentation
=============

For information on building library documentation, please check out
`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
