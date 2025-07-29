This is an R Script that calculates green accessibility around each centroid of a 100x100 m grid. 

## Input
* A 100x100 m vector grid for all built-up gridcells in Hessen with a variable "gen" containing the names of municipalities.
* Three vector layers with low, medium and high green as seperate files for each municipality. These files are outputs of a previously run process. They are named with a certain pattern, containing each municipalities name. 

## Output
* A geopackage for each municipality with green accessibility within a 300 m radius around the centroid of each 100x100 m grid cell.
  * "ha_6" gives the area of high green in hectar within a 300 m radius
  * "ha_5" gives the area of medium green in hectar within a 300 m radius
  * "ha_4" gives the area of low green in hectar within a 300 m radius
* A geopackage for each municipality with green accessibility within a 700 m radius around the centroid of each 100x100 m grid cell.
  * "ha_6" gives the area of high green in hectar within a 700 m radius
  * "ha_5" gives the area of medium green in hectar within a 700 m radius
  * "ha_4" gives the area of low green in hectar within a 700 m radius
    
