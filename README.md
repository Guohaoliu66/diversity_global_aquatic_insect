# Global freshwater insect diversity and drivers

## Overview 
This is a project to explore global freshwater insect diversity and the drivers. Key environmental and anthropogenic factors affecting freshwater insect diversity were revealed by analyzing the diversity of freshwater insects in different regions of the globe (extracted from the EPTO database: https://glowabio.org/project/epto_database/).

## Environmental Requirements 

### Raw data
The EPTO database you can easily download from https://glowabio.org/project/epto_database/.  

### Software Requirements
This project uses the R (verson 4.3.2) for data analysis, so R and some specific R packages need to be installed. 

## Description
All biotic and abiotic data used in this project were obtained from open databases and literature. Please prepare the necessary raw data and R packages prior to analysis, see below:

### Installation
`install.packages(c('dplyr', 'tidyverse', 'vegan', 'lubridate', 'data.table', 'BAT', 'iNEXT.3D', 'ggplot2' 'ggvenn', 'spatialreg', 'spdep'))`

### Additional input data

Global basin boundary data extracted from the HYdroBASIN database of four levels of basin data, see: https://www.hydrosheds.org/products/hydrobasins.  
Global_EPTO_Database.csv extracted from the EPTO database: https://glowabio.org/project/epto_database/.  
Site data: site001-site007 were extracted from the Global_EPTO_Database.csv and the coordinates were connected to the unique HYBAS_ID using QGis software


## Data and code for the paper:
Liu, G., Lin, Z., Soininen, J., Dalu, T., Juvigny-Khenafou, N.P.D., Khan, S., Mu, H., Oduro, C., Qi, X., Qu, X., Riis, T., Wijewardenec, L., Zhang, M., Li, J., Wu, Y. & Wu, N. 2025. Standardized diversity estimation uncovers global distribution patterns and drivers of stream insects. npj Biodiversity, in press.
