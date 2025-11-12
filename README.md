# Blackouts in the Texas Winter Storms

## Purpose of this project

This project investigates the impacts of the February 2021 Texas power crisis, which occurred during a series of severe winter storms that swept across the United States from February 10–20, 2021. The crisis left millions of Texans without power in freezing temperatures, revealing vulnerabilities in the state’s energy infrastructure and raising questions about equity in disaster impacts and recovery.

The analysis focuses on estimating the number of homes in the Houston metropolitan area that lost power during the event and examines whether these impacts were disproportionately felt across socioeconomic groups. Using remotely-sensed night lights data and demographic information, this project connects environmental, infrastructural, and social data to explore the intersection between climate change, infrastructure resilience, and environmental justice.

## Repository Structure

``` bash
texas-power-crisis
└───README.md
└───Rmd/Proj files    
└─── texas-power-crisis.qmd
└───.gitignore
    └───data
        └───gis_osm_buildings_a_free_1.gpkg
        └───gis_osm_roads_free_1.gpkg
        └───ACS_2019_5YR_TRACT_48_TEXAS.gdb
            └───census tract gdb files
        └───VNP46A1
            └───VIIRS data files
```

## Data Access

This project uses publicly available spatial and remote sensing data sets stored locally within the repository under the `data/` directory.

VIIRS Nighttime Lights (VNP46A1) data are obtained from the Visible Infrared Imaging Radiometer Suite (VIIRS) on-board the Suomi satellite. These data provide daily measurements of nighttime light intensity, allowing detection of power outages by comparing pre-storm and post-storm brightness levels. The data set is distributed by [NASA’s Earth Observing System Data and Information System](https://www.earthdata.nasa.gov/).

OpenStreetMap data on buildings and roads are used to spatially identify residential areas and estimate the number of homes affected by outages. Data can be accessed through Geofabrik’s [download](https://download.geofabrik.de/) site of OpenStreetMap.

U.S. Census Bureau ACS (2019 5-Year Estimates) data provide demographic and socioeconomic variables at the census tract level for the state of Texas. These data are used to investigate potential disparities in outage impacts and recovery patterns. The data set is available via the [U.S. Census Bureau](https://www.census.gov/).

## Authorship

-   The project author: **Jay Kim**
-   Instructor: **Annie Adams**
-   Teaching Assistant: **Ale Vidal Meza**

## Reference

Texas Tribune. (2021). “Texas power grid failure: How it happened.” The Texas Tribune.

National Oceanic and Atmospheric Administration. (2021). February 2021 Winter Storm Event Summary.

OpenStreetMap contributors. (2021). OpenStreetMap data (buildings and roads). Retrieved from <https://www.openstreetmap.org>

NASA Earth Observing System Data and Information System (EOSDIS). (2021). VIIRS VNP46A1 Nighttime Lights Data. Retrieved from <https://earthdata.nasa.gov/>

U.S. Census Bureau. (2019). American Community Survey 5-Year Estimates (ACS 2019).
