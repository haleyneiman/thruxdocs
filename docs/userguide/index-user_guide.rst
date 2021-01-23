.. _User-Guide:

**Signing In**
================

Once the application is open, sign in with your account.

.. figure:: images/SignIn.PNG
    :align: center
    
    Sign In at the Top Right

**Navigating THRUX**
====================

.. _Workspace-Toolbar:

#################
Workspace Toolbar
#################

The left-side toolbar is the Workspace Toolbar.  The purple shading indicates an open and active Workspace, while grey shading only indicates an open Workspace.  

.. figure:: images/workspace-toolbar-1.PNG
    :align: center

    Workspace Toolbar

Workspaces can be detached to separate windows by clicking and dragging the Workspace's icon in the Workspace toolbar.  

These windows can be docked by clicking Dock in the top right of the undocked window.

.. figure:: images/workspace-toolbar-dock.PNG
    :align: center

    Docked One-Line separate from the main application

.. figure:: images/workspace_docking.PNG
    :align: center

    Docking Workspaces allows Workspaces to be viewed on multiple monitors

################
Explorer Toolbar
################

Explorers and other Utility tools can be found on the :ref:`Explorer Toolbar <Explorer-Toolbar>` on the right-side toolbar.  These tools can be pinned to always be visible (pin icon).

.. figure:: images/explorer-toolbar-1.PNG
    :align: center

    Using the :ref:`Properties Explorer <Properties-Explorer>` and :ref:`Flag Tracker <Flag-Tracker>` while working in the :ref:`One-Line <One-Line>` Workspace

.. _Navigation-Bar:

##################
Navigation Bar
##################

Designers have the ability to search for anything within the model.

For example, if searching for a piece of Equipment, simply type the name.

Options will be displayed where something is found.  
 
.. figure:: images/navigation_bar-1.PNG
    :align: center

    Navigation Bar

Selection will navigate you to the location within the application.

.. figure:: images/navigation_bar-2.PNG
    :align: center

    Navigating to the Schedule for MDB-1

####################
Additional Commands
####################

Zoom Extents allows the user to quickly pan to the center of the screen.  Double click the mouse wheel to Zoom Extents.

.. index:: Getting Started

**Creating a New Project**
==========================

Click the Home button, and then the Add (+) button to create a new Project.

.. figure:: projectsettings/images/new_project-1.PNG
    :align: center

    The Home Screen is a Project portal that provides quick access to recent Projects

##############################
Opening an Existing Project
##############################

Existing projects or recently opened projects are shown below the Open Project section.

.. figure:: projectsettings/images/open_project-1.PNG
    :align: center

    Check the recently opened lists to pick up where you left off

.. _Project-Settings:

################
Project Settings
################

Project Settings are a set of customizable parameters on which to base the design.

.. figure:: projectsettings/images/project_settings-1.PNG
    :align: center

    Project Settings are accessible by clicking on File, and then Settings

.. toctree::
    :maxdepth: 2

    projectsettings/defaultmodelparameters/index-default_model_parameters
    projectsettings/calculationsettings/index-calculation_settings
    projectsettings/autosizingfilters/index-auto_sizing_filters
    projectsettings/flagsettings/index-flag_settings
    projectsettings/customdesignassistancesettings/index-custom_design_assistance_settings
    projectsettings/laborrates/index-labor_rates

##############
Roadmap
##############

To help guide the design process, refer to the Roadmap.  Clicking on each node will bring you to that process.

.. figure:: images/Roadmap.PNG
    :align: center

    Roadmap

.. _Architectural-Workspaces:

**Defining Architectural Elements**
===================================

###################
Overview
###################

The goal of the Architectural Workspaces, :ref:`Floor Plans <Floor-Plans>` and :ref:`Arch. Elements <Arch.-Elements>`, is to provide a way for you to quickly mass the load of a building.  These locations aid with point-to-point calculations such as voltage drop.

However, these Workspaces are completely optional.  For a smaller project, you may not find it necessary to set up these Workspaces and instead, find it faster to manually input feeder lengths in the :ref:`One-Line <One-Line>`.  

This information can be :ref:`imported <Revit-Interoperability>` from an Architectural Revit model.

The :ref:`Arch. Elements <Arch.-Elements>` Workspace allows you to modify the architectural elements of the model.  Here, it is possible to modify other characteristics of a Floor.  For example, when massing the load of a building, you may want to assign a load requirement or load density to each Floor.  This load is based off of the Floor's Space Type.

These elements can be created in the :ref:`Floor Plans <Floor-Plans>` Workspace, or the :ref:`Architectural Elements <Arch.-Elements>` Workspace.

Equipment Distances
-------------------

.. _Calculated-Length:

^^^^^^^^^^^^^^^^^^^^^^^^
Calculated Length
^^^^^^^^^^^^^^^^^^^^^^^^

Distances between Equipment are determined by their respective Room locations.  Calc. Length (Calculated) represents the distance between two Rooms via an orthogonal route.

The vertical distance between Rooms is the difference between their respective elevations.

.. figure:: images/equipment_distances-1.PNG
    :align: center

    Route between Rooms on the same Floor, and vertical distance between stacked Rooms

It is often necessary to offset through a Riser.  The total distance or :ref:`Net Length <Net-Length>` is determined by the centerpoints of the respective entities.

.. figure:: images/equipment_distances-2.PNG
    :align: center

    Routing from Room A, through Riser A, and terminating at Room B

.. _Manual-Added-Length:

^^^^^^^^^^^^^^^^^^^^^^^^
Manual Added Length
^^^^^^^^^^^^^^^^^^^^^^^^

Manual Added Length is an additional factor which is added to a circuit's :ref:`Calc. Length <Calculated-Length>` property and is a customizable default setting.  See :ref:`here <Default-Model-Parameters>` for more information.

.. _Net-Length:

^^^^^^^^^^^^^^^^^^^^^^^^
Net Length
^^^^^^^^^^^^^^^^^^^^^^^^

The Net Length is composed of the :ref:`Calc. Length <Calculated-Length>` and the :ref:`Manual Added Length <Manual-Added-Length>`.

Loading System
-------------------

The Architectural Elements are the unifying components which Engineers base their design.  However, various engineering disciplines refine and base their calculations off of different elements.

You have the ability to abstract the architectural elements of a model to create Load Packages.  Ideally these entities would be abstracted away from a Revit model.  However, during the early stages of development, a Revit model may not exist.

Creation of these architectural entities allow for the THRUX engine to fully utilize its Loading System which applies loading factors dictated by the designer and the Project's applicable safety codes and standards.

.. figure:: images/loading_system-1.PNG
    :align: center

    Creating Architectural Packages to model loads

Modeling residential loads relies on creating entities that are based off of the NEC.

.. figure:: images/loading_system-2.PNG
    :align: center

    Creating Architectural Packages to model residential loads

Groups of architectural entities can be created within THRUX, or imported from a Revit model.  Ultimately, Architectural Packages are loads that can be attached to Equipment.

.. _Floor-Plans-Overview:

############
Floor Plans
############

The :doc:`Floor Plans <definingarchitecturalelements/floorplans/index-floor-plans>` Workspace is a 2-D representation of the Project and is used to model locations of Equipment.  

.. toctree::
    :maxdepth: 3

    definingarchitecturalelements/floorplans/index-floor-plans

#######################
Architectural Elements
#######################

:doc:`Arch. Elements <definingarchitecturalelements/archelements/index-arch-elements>` are a tabular representation of the Architectural entities of the model.  

.. toctree::
    :maxdepth: 3

    definingarchitecturalelements/archelements/index-arch-elements

.. _Electrical-Workspaces:

**Building the Electrical Model**
=================================

###################
Overview
###################

There are three (3) main Workspaces to build the electrical system.  

These include: :ref:`Riser <Riser>`, :ref:`One-Line <One-Line>`, :ref:`Schedules <Schedules>`.  

Reports of a model can be generated at any time using the :ref:`Studies <Studies>` Workspace.  

Hosted vs. Unhosted Systems
--------------------------- 

If a piece of Equipment is not fed from a source, then it is designated as Unhosted.  During the stages of design, it is common to model hypothetical scenarios before all information is known.  For example, as part of a larger project, an Architect may decide to create a space dedicated for a computer lab, but not yet decide on its exact location.  While the location is not yet finalized, you can still model an Unhosted System with the intent of attaching the system to the main network in the future.  Modeling Unhosted Systems allows flexibility when the source of a network is not yet known or if you want to create segregated distribution networks and tie them together at a later time.

####################
Riser
####################

.. toctree::
    :maxdepth: 2

    buildingelectricalmodel/riser/index-riser 

####################
One-Line
####################

.. toctree::
    :maxdepth: 2

    buildingelectricalmodel/one-line/index-one-line


####################
Schedules
####################

.. toctree::
    :maxdepth: 2

    buildingelectricalmodel/schedules/index-schedules

####################
Flag Tracker
####################

.. toctree::
    :maxdepth: 2

    buildingelectricalmodel/flagtracker/index-flag_tracker

####################
Studies
####################

.. toctree::
    :maxdepth: 2

    buildingelectricalmodel/studies/index-studies

**Building the Mechanical Model**
=================================

Coming soon!

.. toctree::
    :maxdepth: 2

    buildingmechanicalmodel/index-building_mechanical_model

**Building the Plumbing and Fire Protection Model**
====================================================

Coming soon!

.. toctree::
    :maxdepth: 2

    buildingpfpmodel/index-building_pfp_model

.. _Pricing-Model:

**Pricing Model**
====================

The Pricing Model is built around the Electrical model and can be viewed in a few Workspaces.  The :ref:`Price Tracker <Price-Tracker>` is used to live monitor the price of the model.  For example, as you change the location of a major equipment room, the Price Tracker would display order of magnitude estimates for that change.  For a more complete tabular report, use the :ref:`Pricing Report <Pricing-Report>` Workspace.

:ref:`Equipment Rates <Equipment-Rates>` is a customizable catalog which composes the bid for materials.
 
.. toctree::
    :maxdepth: 3

    pricingmodel/pricingreport/index-pricing_report
    pricingmodel/pricetracker/index-price_tracker
    pricingmodel/equipmentrates/index-equipment_rates

.. _Project-Management:

**Project Management**
======================

Engineers are often tasked to study different alternatives or schemes and present them to the Owner.  

The :ref:`Issuance Log <Issuance-Log>` allows you to create Branches, while the :ref:`Change Tracking <Change-Tracking>` Workspace allows you to compare Branches against the base Branch.

.. figure:: projectmanagement/images/project_management-1.PNG
    :align: center

    Project Management tools - Issuance Log, Change Tracking

.. toctree::
    :maxdepth: 3

    projectmanagement/issuancelog/index-issuance_log
    projectmanagement/changetracking/index-change_tracking
    projectmanagement/accessibility/index-accessibility

.. _Explorer-Toolbar:

**Explorers and other Utility Tools**
============================================

The right-side toolbar of THRUX is generally where the explorers or utility tools are located.  Explorers can be pinned to always be visible while other explorers are being used.

.. figure:: explorersandutilitytools/images/explorersandutilitytools-1.PNG
    :align: center

    Explorer Toolbar

.. toctree::
    :maxdepth: 2

    explorersandutilitytools/propertiesexplorer/index-properties_explorer
    explorersandutilitytools/cascademonitor/index-cascade_monitor
    explorersandutilitytools/dataexporter/index-data_exporter
    explorersandutilitytools/codesreference/index-codes_reference
    explorersandutilitytools/statusbar/index-status_bar

.. _Recovery-Options:

**Recovery Options**
====================

THRUX models are stored in the cloud and are periodically backed up. You can revert a model to a previous point in time via the Open Project window. Select your project and use the Restore command on the model you wish to roll back.

.. figure:: recoveryoptions/images/restore-2.PNG
    :align: center

.. _Release-Data:

**Automatic Updates**
=====================

Whenever THRUX is opened, it automatically searches for updates.  

Refer to the Version Number in the bottom right of the :ref:`Status Bar <Status-Bar>`. 

.. figure:: automaticupdates/images/version.PNG
    :align: center

To see an outline of updates between each Version, click on the information icon located in the top-right of the top menu bar. 

.. figure:: automaticupdates/images/release_data-1.PNG
    :align: center

Use the arrows to navigate between each Version.

.. figure:: automaticupdates/images/release_data-2.PNG
    :align: center

.. _Revit-Interoperability:

**Revit Interoperability**
==========================

The Architectural information which comprise the Architectural Workspaces, :ref:`Arch. Elements <Arch.-Elements>` and the :ref:`Floor Plans <Floor-Plans>`, can be imported from a Revit model.

In addition, a THRUX model can be exported to Revit.  You can then fine-tune Equipment locations using Revit, and verify the integrity of the design using THRUX.

.. figure:: definingarchitecturalelements/images/revit-interop-1.PNG
    :align: center

.. _AutoCAD-Interoperability:

**AutoCAD Interoperability**
============================

:ref:`Schedules <Schedules>` are exportable to AutoCAD or Excel.

.. figure:: buildingelectricalmodel/schedules/images/schedules-exporting-1.PNG
    :align: center

    Exporting Schedules to AutoCAD

.. figure:: buildingelectricalmodel/schedules/images/schedules-exporting-2.PNG
    :align: center

    Exporting Schedules to AutoCAD