# Global freshwater insect diversity and its drivers

## Project Overview 
This is a project to explore global freshwater insect diversity and the drivers behind it. Key environmental and anthropogenic factors affecting freshwater insect diversity were revealed by analyzing the diversity of freshwater insects in different regions of the globe (extracted from the EPTO database: https://glowabio.org/project/epto_database/).

## Environmental Requirements 

### Hardware Requirements
Because of the size of the EPTO database (Approx. 3.2GB), a standard computer with enough memory to support user-defined operations is required. We recommend a computer with the following specifications:
Memory: 16+ GB
CPU: 4+ cores

### Software Requirements
This project uses the R (verson 4.3.2) for data analysis, so R and some specific R packages need to be installed. 

## Description
All biotic and abiotic data used in this project were obtained from open databases and literature. Please prepare the necessary raw data and R packages prior to analysis, see below:

### Installation
`install.packages(c('dplyr', 'tidyverse', 'vegan', 'lubridate', 'data.table', 'BAT', 'iNEXT.3D', 'ggplot2' 'ggvenn', 'spatialreg', 'spdep'))`

### Additional input data
Global basin boundary data extracted from the HYdroBASIN database of four levels of basin data, see: https://www.hydrosheds.org/products/hydrobasins.

## Expected output
We can obtain a global pattern of geographic distribution of aquatic insect diversity (including basin, latitude and freshwater major habit type) and its drives. 
By running these R codes, we can repeat almost all of the results from the study. Note, however: due to the uncontrolled standard error when using the iNEXT.3D package for diversity calculations, it is almost impossible to reproduce exactly the same results (the ratio of observed to normalized diversity), even though we set the parameter nboot = 50 for more reliable results
