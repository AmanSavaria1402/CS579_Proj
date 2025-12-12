This is the repository for the project __Ridership Prediction for Expanding Metro
Networks__ for CS-579. The repository contains all the code, the data used and the trained models.

The code is present in 3 different jupyter notebooks. They are as follows:
- exploration: This notebook contains code for creating the graph for the CTA-L network from the shapefiles available in the chicago data portal.
- Graph_Data_Collection: This notebook creates the features for all the 3 categories for the entire graph and saves it to disc.
- DataCreation-Graph_Structure_Temporal: The notebook above created all the features but the network structure features created by it was for only the latest graph. This notebook creates these features for all the different 'period' graphs.
- Model_Training: This notebook finally concatenates all the features to create the training data. It then trains the Neural Network and finally predicts for the three stations (Damen, Lawrence and Berwyn).

#### Note about the files shapefiles:
The shapefiles are also provided in the repo, however, the census blocks shapefile, which contains the shapefiles for all the block groups in the state of IL, is too large and may have not been uploaded correctly while pushing due to space constraints. Just to be safe, please download the shapefiles for all the blockgroups in Illinois from [here](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html).