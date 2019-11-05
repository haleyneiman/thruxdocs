.. _Status-Bar:

Status Bar
----------

The bottom left of the Status Bar indicates the state of THRUX.  It will change colors as the state changes.

The bottom right of the Status Bar provides a few more Utility functions such as the ability to Design Assistance, Refreshing Calculations, Auto Calculate, and Toggle Flag Settings.

.. _Design-Assistance:

#################
Design Assistance
#################

Different Design Mode Levels are togglable in THRUX, which are indicated by the three lightning symbols.  The default mode is Full Design Assistance which references the applicable safety codes, standards, and user settings to calculate code-minimum values.

*******************************************************************************************************************************************************************************************************************************************************************************************

.. _Full-Design-Assistance:

Full Design Assistance
+++++++++++++++++++++++

Any change in circuit properties will trigger a recalculation in all relevant code-minimum values.

.. figure:: images/status_bar_utility_1.PNG
    :align: center

.. _Custom-Design-Assistance:

Custom Design Assistance
+++++++++++++++++++++++++

Any change in circuit properties will trigger a recalculation in all relevant code-minimum values that are not omitted by the Custom-Design-Assistance Settings.  Flags will still be raised as long as they are enabled.

.. figure:: images/status_bar_utility_2.PNG
    :align: center

.. _No-Design-Assistance:

No Design Assistance
++++++++++++++++++++

Designer has full manual control of all circuit properties.  No auto-sizing will be performed.

.. figure:: images/status_bar_utility_3.PNG
    :align: center

*******************************************************************************************************************************************************************************************************************************************************************************************

.. _Force-Calculation-Refresh:

Force Calculation Refresh
+++++++++++++++++++++++++
Refreshes all calculations on the active Workspace.

.. figure:: images/status_bar_utility_4.PNG
    :align: center

    Force Calculation Refresh

.. _Auto-Calulate:

Auto Calculate
+++++++++++++++++++++++++
Toggles the calculation engine on or off.

Changing circuit properties will cause recalculations in a variety of areas.  This can be an expensive process and can cause the application to slow down.

This may not be appropriate during a presentation.  

Turning off the calculation engine enables the designer to stop this process.

.. figure:: images/status_bar_utility_5.PNG
    :align: center

    Auto Calculate - Off

.. index:: Is there a way to Disable all Flags?

.. _Toggle-Flags:

Toggle Flags
+++++++++++++++++++++++++

The Toggle Flags button will toggle the visibility settings of all Flags.  

.. figure:: images/status_bar_utility_6.PNG
    :align: center

    Flags - Off

.. _Version:

Version
+++++++
Tracks the current version of THRUX.