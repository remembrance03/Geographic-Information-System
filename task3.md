# Task 3: Population Data Collection and Integration

### Objective
### The objective of this task is to collect municipality-wise population data for the selected district, clean and standardize the dataset, and integrate it with the municipality boundary layer for further GIS analysis.

---

### Step 1: Download Population Data

1. Open a web browser and visit:
    https://www.citypopulation.de

2. Navigate to the population data section for Nepal.

Download municipality-wise population data for the selected district.

Save the dataset in the project workspace (outside the file geodatabase).

Step 2: Clean and Prepare Population Data

Open the population dataset in Excel or a similar spreadsheet tool.

Ensure that municipality names exactly match those in the municipality boundary layer.

Remove unnecessary columns and keep only the following fields:

District Name

Municipality Name

Municipality Status (Metro / Sub-metro / Municipality / Rural Municipality)

Population 2011

Population 2021

Check for spelling differences, extra spaces, or formatting issues and correct them.

Save the cleaned table in a compatible format (e.g., .xlsx or .csv).

Step 3: Add Population Table to ArcGIS

Open ArcMap or ArcGIS Pro.

Add the cleaned population table to the map.

Verify that the attribute table loads correctly and that all required fields are present.

Step 4: Export Municipality Boundary Layer for Joining

To ensure a stable and editable join, the municipality boundary layer was exported before performing the attribute join.

Right-click the municipality boundary layer.

Select Data → Export Features.

Save the exported feature class inside:
Kavrepalanchowk_Panchkhal_2278639.gdb → Kavrepalanchowk feature dataset

Use this exported layer for the population data join.

Step 5: Join Population Data with Municipality Boundaries

Right-click the exported municipality boundary layer.

Select Joins and Relates → Join.

Set the join parameters:

Join Field (Layer): Municipality name

Join Table: Cleaned population table

Join Field (Table): Municipality name

Run the join and verify that population fields are correctly appended to the attribute table.

Step 6: Verify Join and Save Outputs

Open the attribute table of the joined layer.

Confirm that population values for 2011 and 2021 are correctly linked to each municipality.

Save the final joined layer inside the Kavrepalanchowk feature dataset for use in further GIS analysis and thematic mapping.