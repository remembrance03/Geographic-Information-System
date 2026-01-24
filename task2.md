Task 2: Administrative Boundary Data Processing
Objective

The objective of this task is to extract administrative boundaries for the selected district and municipality and organize them properly for further GIS analysis.

Step 1: Download Administrative Boundary Data

Open a web browser and go to:
https://nationalgeoportal.gov.np

Download the Nepal Local Units Administrative Boundary (1:1,000,000) dataset.

Extract the downloaded files to your project workspace.

Step 2: Add Data to ArcGIS

Open ArcMap / ArcGIS Pro.

Add the administrative boundary shapefile to the map.

Verify that the layer contains district and municipality attributes.

Step 3: Extract Municipality Data Using Split by Attribute

Open ArcToolbox.

Navigate to:
Data Management Tools → General → Split

Select Split By Attributes.

Set:

Input Feature: Local Units administrative boundary layer

Split Field: District name field

Output Workspace:
Kavrepalanchowk_Panchkhal_2278639.gdb → Kavrepalanchowk feature dataset

Run the tool to extract municipality layers for the selected district.

Step 4: Create a District Boundary Using Dissolve

Open ArcToolbox.

Navigate to:
Data Management Tools → Generalization → Dissolve

Set:

Input Features: Municipality boundary layer of Kavrepalanchowk

Dissolve Field: District name

Run the tool to generate a single district boundary.

Step 5: Organize Outputs

All extracted municipality boundaries and the dissolved district boundary are stored inside the Kavrepalanchowk feature dataset within the project geodatabase. This ensures proper data organization and spatial consistency for subsequent analysis.