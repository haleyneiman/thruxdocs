.. _Revit_Interop_Arch_Import:

########################################
Import an Architectural Model from REVIT
########################################

Link an architectural revit model to THRUX. 

1. Login to the THRUX `Account Portal <http://thruxcoreweb.azurewebsites.net/AccountPortal>`_.
2. Navigate to the downloads section. Download and install the THRUX REVIT add-in for the required version of REVIT.
3. Open REVIT, you should see the THRUX add-in available on the ribbon. 
4. Open the model you would like to export. Make sure all applicable REVIT links are loaded into the model. Ex, if the building exterior (or curtain wall) is captured in a separate model from the core of the building make sure both models are loaded. 
5. Select the add-in on the ribbon and select "Export Arch". 
6. A pop up will allow you to select which entity types to export and which phase to include. 

.. figure:: images/RevitImport.PNG
    :align: center
    :alt: revit import

Note - Pay attention to the phases being exported. Exporting non-applicable phases may result in overlapping rooms in THRUX.

7. Select "Export" and save the export file to your desktop. 
8. Run THRUX, open the applicable project, select REVIT from the top ribbon and select "Import Arch Model".

.. figure:: images/RevitToTHRUX.JPG
    :align: center
    :alt: import revit to THRUX

9. An import pop-up will appear, indicating the new elements that are being imported from the architectural model. If the model had been previously imported, this pop up will indcate any changes between this import and the last. 

The next time the same model is imported, changes will be flagged in the new model against what currently exists in THRUX. 


