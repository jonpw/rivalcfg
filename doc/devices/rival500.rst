SteelSeries Rival 500
=====================


Supported Models
----------------

.. rivalcfg_device_family:: rival500


Command-Line Usage
------------------

.. rivalcfg_device_cli:: rival500


Colors
------

This mouse supports colors. Various formats are supported.

.. include:: ./_colors.rst


RGB Gradients
-------------

.. include:: ./_rgbgradient.rst


Buttons
-------

.. figure:: ./images/rival_500_buttons.svg
   :alt: Rival 500 buttons schema

.. include:: ./_buttons.rst


Tactile Alerts
--------------

The Rival 500 has a vibration motor. You can play one of its tactile alerts
with the ``--tactile-alert`` option::

    rivalcfg --tactile-alert buzz

Available alerts are the ones provided by SteelSeries Engine: ``strong-click``,
``sharp-click``, ``soft-bump``, ``double-click``, ``short-double-click``,
``triple-click``, ``buzz``, ``long-buzz``, ``sharp-tick``, ``pulsing``,
``slow-heartbeat``, ``fast-heartbeat`` and ``sad-trombone``.

Playing a tactile alert is an action, not a setting: it is not reset by
``--reset`` and, when used alone, does not write anything to the internal
memory of the mouse.

From Python::

    import rivalcfg

    mouse = rivalcfg.get_first_mouse()
    mouse.set_tactile_alert("double-click")


Python API
----------

TODO
