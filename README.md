# CLEWs-ZMB-2024
 A CLEWs-Based Approach to the Climate-Water-Energy-Food Nexus in Zambia: Enhancing Policy Coherence for Sustainable Development in Zambia

## Introduction

GeoCLEWs_ZM offers a comprehensive set of features to process high-resolution land and water data for Climate, Land, Energy, and Water Systems (CLEWs) modeling. This script (adapted from [Yalda Saedi](https://github.com/YSaedi)) automates data collection from GAEZ v4 and FAOSTAT, processing agro-climatic potential yield, crop water deficit, precipitation, and land cover. Outputs can be combined with electricity information for detailed CLEWs modeling, providing an efficient solution without complex spatial processing. GeoCLEWs_ZM has been successfully tested on Windows machines. Please follow the instructions below to set up and use GeoCLEWs_ZM effectively.

## Creating and Activating the Environment
Ensure all necessary Python packages and dependencies are installed using the provided 'environment.yml' file: 

```bash
conda env create -f environment.yml
conda activate GeoCLEWs
```

## Download Files and Data

1. **CLEWs-ZMB-2024 Folder**: Download the 'CLEWs-ZMB-2024' folder, which includes:

     * **GeoCLEWs.ipynb**: Jupyter Notebook code for running GeoCLEWs.
     * GAEZ and FAOSTAT resources in CSV format.

     * 'Data' folder corresponding to input and output data.

2. **Administrative Boundary Shapefiles**: Download shapefiles for administrative boundaries from GADM or any other sources. Place the file inside the 'Data/input' directory and rename it to "..._ adm0" where "..." represents the 3-letter ISO country code (e.g., "ZMB_adm0.shp" for Zambia).

3. **Clustering Shapefile**: Obtain the required shapefile for clustering from GADM or other sources and store it in the 'Data/input' folder. Rename the files to match the 3-letter ISO country code of your case study, such as "ZMB_data.shp" for Zambia.

Please ensure all necessary files, such as .shx, .shp, etc., are included. For example, for Zambia, include files like ZMB_adm1.dbf, ZMB_adm1.cpg, ZMB_adm1.prj, ZMB_adm1.shp, ZMB_adm1.shx, etc.

## Outputs

GeoCLEWs produces the following outputs:

+ Tabular results in CSV format compatible with clews for CLEWs modeling using OSeMOSYS.
+ Interactive graphs for visualization and analysis.

The units presented in the outputs are recalculated based on the CLEWs framework for consistency and comparability. The outputs provide insights into agro-climatic potential yield, crop water deficit, precipitation, crop evapotranspiration, and land cover, facilitating informed decision-making for sustainable development in Zambia.

