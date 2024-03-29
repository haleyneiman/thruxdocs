.. _Load_Outputs:

########################
Review Load Calc Results
########################

Review the results of calculations in the Load Output workspace. 


.. figure:: images/loadOutput.JPG
    :align: center
    :alt: Load Output

    Review Load Calculations
    
When the Load Outputs workspace is first opened, the System's Browser will automatically open and dock to the right side of the screen. This browser displays all linkable system components in the model. These can be spaces, zones, generic loads or pieces of equipment. Spaces and Zones are broken out into four separate load components: 

* Cooling Load
* Cooling Ventilation Load
* Heating Load
* Heating Ventilation Load

Each component type can be toggled on/off in the System's Browser by using the toggles (shown below). 

.. figure:: images/loadoutputtoggles.png
    :align: center
    :alt: System's Browser Toggles

Select a component to view the associated load visualized in a pie chart. 

Calculated Values
-----------------

**Design CFM** :  Calculated by taking the greatest of four calculation methods

* Sensible Driven CFM - flowrate required to meet sensible load requirements
* Latent Driven CFM - flowrate required to meet latent load requirements
* ACH Driven CFM - flowrate required to meet any applicable ACH requirements for the spaces
* OA Driven CFM - flowrate required to meet any ventilation requirements for the spaces

Note - if any calculation method other than sensible driven CFM is used to determine the design flowrate, reheat will be required to prevent overcooling of the space. 


