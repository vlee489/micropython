.. _install-dev:

============
Installation
============

This section will help you set up the tools and programs needed for
developing programs and firmware to flash to the BBC micro:bit using MicroPython.

Dependencies
------------


Development Environment
-----------------------

You will need:

* git
* yotta

Depending on your operating system, the installation instructions vary. Use
the installation scenario that best suits your system.

Installation Scenarios
----------------------

* :ref:`Windows <microbit-windows>`
* :ref:`OS X <microbit-osx>`
* :ref:`Linux <microbit-linux>`
* :ref:`Debian and Ubuntu <microbit-debian-ubuntu>`
* :ref:`Red Hat Fedora/CentOS <microbit-redhat>`
* :ref:`Raspberry Pi <microbit-rpi>`


.. _microbit-windows:

Windows
~~~~~~~

.. note::

    Current you are unable to build the firmware for Micropython for the
    BBC Microbit due and issue with Yotta!

When installing `Yotta
<http://yottadocs.mbed.com/#installing>`_, make sure you have these components ticked to install.

- `Python <https://www.python.org/downloads/release/python-279/>`_
- `GCC <https://launchpad.net/gcc-arm-embedded/+download>`_
- `CMake <https://cmake.org>`_
- `Ninja <https://github.com/martine/ninja/releases/download/v1.5.3/ninja-win.zip>`_
- `Yotta <http://yottadocs.mbed.com/#installing>`_
- `Git-SCM <https://git-scm.com>`_
- `mbed serial driver <https://developer.mbed.org/handbook/Windows-serial-configuration>`_

You may need to manually added each item's bin folder from Yotta in the PATH system variables.
You'll need to do this if Yotta brings up that some prerequisites are not found when building.

If manually adding the path from the items installed by Yotta doesn't work you may need to download
the required program manually, install them and find their install location and add them to the
PATH system variables


.. _microbit-osx:

OS X
~~~~


.. _microbit-linux:

Linux
~~~~~

These steps will cover the basic flavors of Linux and working with the
micro:bit and MicroPython. See also the specific sections for Raspberry Pi,
Debian/Ubuntu, and Red Hat Fedora/Centos.


.. _microbit-debian-ubuntu:

Debian and Ubuntu
^^^^^^^^^^^^^^^^^

::

  sudo add-apt-repository -y ppa:terry.guo/gcc-arm-embedded
  sudo add-apt-repository -y ppa:pmiller-opensource/ppa
  sudo apt-get update
  sudo apt-get install cmake ninja-build gcc-arm-none-eabi srecord
  pip3 install yotta


.. _microbit-redhat:

Red Hat Fedora/CentOS
^^^^^^^^^^^^^^^^^^^^^


.. _microbit-rpi:

Raspberry Pi
^^^^^^^^^^^^



.. _next-steps:

Next steps
----------

Congratulations. You have installed your development environment and are ready to
begin :ref:`flashing firmware <flashfirmware>`  to the micro:bit.
