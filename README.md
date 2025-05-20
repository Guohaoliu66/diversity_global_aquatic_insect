# Global freshwater insect diversity and drivers

## Project Overview 
This is a project to explore global freshwater insect diversity and the drivers. Key environmental and anthropogenic factors affecting freshwater insect diversity were revealed by analyzing the diversity of freshwater insects in different regions of the globe (extracted from the EPTO database: https://glowabio.org/project/epto_database/).

## Environmental Requirements 

### Raw data
Because of the size of the EPTO database (Approx. 3.2GB), I don't store it here, but you can easily download it from https://glowabio.org/project/epto_database/.  

### Software Requirements
This project uses the R (verson 4.3.2) for data analysis, so R and some specific R packages need to be installed. 

## Description
All biotic and abiotic data used in this project were obtained from open databases and literature. Please prepare the necessary raw data and R packages prior to analysis, see below:

### Installation
`install.packages(c('dplyr', 'tidyverse', 'vegan', 'lubridate', 'data.table', 'BAT', 'iNEXT.3D', 'ggplot2' 'ggvenn', 'spatialreg', 'spdep'))`

### Additional input data

Global basin boundary data extracted from the HYdroBASIN database of four levels of basin data, see: https://www.hydrosheds.org/products/hydrobasins.  
Global_EPTO_Database.csv extracted from the EPTO database: https://glowabio.org/project/epto_database/.  
Site data: site001-site007 were extracted from the Global_EPTO_Database.csv and the coordinates were connected to the unique HYBAS_ID using Qgis software

## Expected output
We can obtain a global pattern of geographic distribution of aquatic insect diversity (including basin, latitude and freshwater major habit type) and its drives.  
By running these R codes, we can repeat almost all of the results from the study. Note, however: due to the uncontrolled standard error when using the iNEXT.3D package for diversity calculations, it is almost impossible to reproduce exactly the same results (the ratio of observed to normalized diversity), even though we set the parameter nboot = 50 for more reliable results.

###  Operation Guide
1. Detailed runtime instructions are included in each file in r_scripts.  
2. Note that I used ArcMap to make Fig.2, Fig.4 ABCDEF, Extended Fig.S1, S3 and S4.  
