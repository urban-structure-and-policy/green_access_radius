This is an R Script that calculates green accessibility around each centroid of a 100x100 m grid. 

## Input
* A 100x100 m vector grid for all built-up gridcells in Hessen with a variable "gen" containing the names of municipalities.
* Three vector layers with low, medium and high green as seperate files for each municipality. These files are outputs of a previously run process. They are named with a certain pattern, containing each municipalities name. 

## Processing
* Clone repo
* Open [green_accessibility_run_all_mun.Rmd](https://github.com/urban-structure-and-policy/green_access_radius/blob/main/green_accessibility_run_all_mun.Rmd)
* Update input/output pahts
* Run all or knit document

## Output
* A geopackage for each municipality with green accessibility within a 300 m radius around the centroid of each 100x100 m grid cell.
  * "ha_6" gives the area of high green in hectar within a 300 m radius
  * "ha_5" gives the area of medium green in hectar within a 300 m radius
  * "ha_4" gives the area of low green in hectar within a 300 m radius
* A geopackage for each municipality with green accessibility within a 700 m radius around the centroid of each 100x100 m grid cell.
  * "ha_6" gives the area of high green in hectar within a 700 m radius
  * "ha_5" gives the area of medium green in hectar within a 700 m radius
  * "ha_4" gives the area of low green in hectar within a 700 m radius
    
## Tested with the following R version and packages
R version 4.4.0 (2024-04-24 ucrt)
Platform: x86_64-w64-mingw32/x64
Running under: Windows 10 x64 (build 19045)

other attached packages:
* lubridate_1.9.3 
* forcats_1.0.0   
* readr_2.1.5     
* tidyr_1.3.1     
* tibble_3.2.1    
* ggplot2_3.5.1   
* tidyverse_2.0.0 
* purrr_1.0.2     
* stringr_1.5.1   
* dplyr_1.1.4    
* sf_1.0-16      
