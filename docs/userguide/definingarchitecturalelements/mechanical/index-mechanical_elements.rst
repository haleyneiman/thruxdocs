:orphan:

.. _Mechanical_Elements:


###################
Mechanical Elements
###################

Space Types
-----------

Mechanical Space Types are templates for the spaces or rooms in the model. Space Types define the loading, temperature setpoints and occupancy types for spaces. 

.. figure:: images/Mechanical_Space_Types.PNG
    :align: center
    :alt: open project

    Mechanical Space Types

.. csv-table:: Space Type Properties
    :file: images/SpaceTypeProperties.csv
    :widths: 30, 70
    :header-rows: 1


Wall Types
----------

Wall Types are templates applied to the walls in project. They specify wall construction characteristics. These templates can be associated to individual walls in the floor plans. 

.. csv-table:: Wall Type Properties
    :file: images/WallTypeProperties.csv
    :widths: 30, 70
    :header-rows: 1


Window Types
------------

Window Types are templates applied to the glazing portion of walls in the project. They specify the glass construction characteristics, as well as the dimensions.

.. csv-table:: Window Type Properties
    :file: images/WindowTypeProperties.csv
    :widths: 30, 70
    :header-rows: 1


Roof Types
----------

Roof Types are templates applied to the roofs in the project. These define the roof construction characteristics. 

.. csv-table:: Roof Type Properties
    :file: images/RoofTypeProperties.csv
    :widths: 30, 70
    :header-rows: 1

Spaces
------

Spaces are rooms, defined and created visually in the floor plans (or imported from REVIT). The elements Space table is a good place to make bulk edits to the properties of multiple spaces at once. More information about space loads can be displayed by toggling on more properties. Many find it helpful to export this table to excel. 

.. csv-table:: Space Properties
    :file: images/SpaceProperties.csv
    :widths: 30,70
    :header-rows: 1


Zone Types
----------

Zone Types define templates for thermal zones and the equipment that serves them. Once a zone is created in the model and a zone type is assigned, a piece of mechanical equipment (defined by the zone type) will be automatically created and linked to zone. Zone types can be used at any stage of the project lifecycle. For example, for block load calculations zone types can be used to create air handlers to serve a full floor. In a fit-out project zone types can be used to automically create terminal units.  

.. csv-table:: Zone type Properties
    :file: images/ZoneTypeProperties.csv
    :widths: 30,70
    :header-rows: 1

Zones
-----

Zones are collections of spaces that thermally controlled together. Zones are created visually in the floor plans. Here you can view the spaces associated with a zone and the resultant load. 

Mechanical Equipment
--------------------

Load carrying equipment in the model. 