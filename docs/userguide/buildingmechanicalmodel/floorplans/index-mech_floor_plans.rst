.. _The-Mechanical-Floor-Plans:

##########################
Working in the Floor Plans
##########################

The mechanical floor plans provide a visual interface for load calculations. Here, the basis of design templates created in the :ref:`Elements Workspace <Mechanical_Elements>` can be associated with the spaces, walls, windows, and roofs in the building.

Follow these :ref:`steps <Floor-Plans>` to import an architectural REVIT model or build a lightweight floor plan in THRUX. 

Assigning Space Types to Spaces
-------------------------------

Double click a space, and the :ref:`Properties Explorer <Properties-Explorer>` will open, displaying information about the selected space. Space types can be assigned one by one using this explorer or, they can be quickly assigned with the Quick Tag tool, shown below. 

.. figure:: images/SpaceTypeQuickTag.PNG
    :align: center
    :alt: quick tag

    Select a space type from the Quick Tag Explorer and click spaces in the floor plans to assign them to the selected template. 

Wall Edit Mode
--------------

While THRUX understands the length, height and direction of every wall in the model, defining a wall as exterior vs. interior is left up to the user. Toggle on "Wall Edit Mode" at the top of workspace to edit the walls of the building.

.. image:: images/WallEditModeScreenshot.png
    :align: center
    :alt: Wall Edit Mode

With Wall Edit Mode enabled, the edges of each space become selectable. To batch select, draw a selection region enclosing one or more of the highlighted edges. Dragging to the left selects every edge touched. Dragging to the right selects only the edges fully enclosed by the region. By default, selected egdes are indicated as exterior and therefore contribute to the load of the space. 

Exterior walls are indicated visually in the plans with highlighted teal. Interior "load contributing" walls are indicated with a soft tan. Note, interior walls separating conditioned spaces are NOT required to be identified and should be left unselected. Only interior walls that separate spaces of differing interior temperature setpoints are required to be indicated as interior.

.. csv-table:: Wall Properties
    :file: images/WallProperties.csv
    :widths: 30, 70
    :header-rows: 1

Global Building Rotation
------------------------

Modify the global building rotation field to align the THRUX grid with the actual building orientation. Building rotation is measured in degrees from North. 

.. image:: images/BuildingRotation.png
    :align: center
    :alt: Global Building rotation

Zone Edit Mode
--------------

Toggle on Zone Edit Mode at the top of the workspace to create, modify and delete thermal zones.

Draw a selection box around multiple spaces to group them together into a zone. Once the zone is created, it can modified and reshaped to encompass other spaces. A zone considers any space fully enclosed by it's boundary to be included in the zone. Moving or reshaping the region will cause any spaces included to highlight.  

.. figure:: images/ZoneEditMode.JPG
    :align: center
    :alt: Create/Modify/Delete zones

    Create/Modify/Delete zones

Floor Slabs and Roofs
---------------------

By default, the floor and roof of a space is assumed to be adjacent to another conditioned space. To indicate that a floor or roof should apply a load to it's respective space, toggle on the "Contains Floor Slab" or "Contains Roof" toggles in the Space properties browser. 

.. figure:: images/FloorSlab.JPG
    :align:center
    :alt: Floor Slab/Roof Toggles

Once toggled on, a new set of properties will appear, applying to the floor slab or roof. 

.. csv-table:: Floor Slab Properties
    :file: images/FloorSlabProperties.csv
    :widths: 30,70
    :header-rows: 1

.. csv-table:: Roof Properties
    :file: images/RoofProperties.csv
    :widths: 30,70
    :header-rows: 1









