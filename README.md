# Lights Out in Houston: Mapping the Effects of Winter Storm Uri

## Description

Winter Storm Uri was a powerful and catastrophic winter storm that devastated several communities in Texas during February 13-17 2021. The state was unprepared for a significant loss of power; power plants and grids were not prepared to handle freezing temperatures coupled with increased electricity usage to heat homes (Zhou et al., 2024). Nearly 246 people perished, 4.5 million homes lost power, and costed the state about \$195 million in damages (Zhou et al., 2024). As such, Winter Storm Uri is listed as the costliest and one of the deadliest natural disasters in Texan history.

The City of Houston, the county’s most populous city, had an estimated population of 2,333,346 in 2023 with a median household income of \$62,894 (DataUSA, n.d.) . The city experienced a population growth of approximately 0.18% and a median household income increase of about 4.06% (DataUSA, n.d.) . Houston was one of several urban centers in Harris County that were significantly affected by the storm and is a key area for analysis.

The purpose of this assignment is to assess the extent to which houses and census tracts in Houston lost power during Winter Storm Uri. The analysis utilizes spatial manipulation between raster and vector types to identify homes in Houston that experienced a blackout, as well as an assessment of median income for census tracts affected by the blackout based on socioeconomic data. The following research question was referenced to guide the analysis:

**To what extent were homes and census tracts in Houston impacted by the power outage caused by Winter Storm Uri?**

## Repository Structure

This repository contains:

```         
Lights Out in Houston: Mapping the Effects of Winter Storm Uri
└───README.md
└───eds-223-hw-3.pdf    
└───eds-223-hw-3.Rproj    
└───Mapping_the_Effects_of_Winter_Storm_Uri.qmd 
└─── figs
     └───Affected_Census_Tracts_Boxplot.png
     └───Affected_Census_Tracts.png
     └───Homes_in_Houston_Affected_by_Blackout.png
     └───median_income_census_tracts.png
     └───post_storm.png
     └───pre_storm.png
└───.gitignore
    └───data
        └───gis_osm_buildings_a_free_1.gpkg
        └───gis_osm_roads_free_1.gpkg
        └───ACS_2019_5YR_TRACT_48_TEXAS.gdb
            └───census tract gdb files
        └───VNP46A1
            └───VIIRS data files
```

## Data Description and Access

VIIRS data, distributed through NASA's [Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center](https://ladsweb.modaps.eosdis.nasa.gov/), were obtained as 10×10 degree tiles for two days surrounding the storm: February 7 and February 16. These dates were selected due to relatively clear skies and minimal cloud cover, making them optimal for assessing night light intensity before and after the storm. Since Houston lies on the border of two tiles (h08v05 and h08v06), both tiles were downloaded for each day and are stored in the `VNP46A1` folder.

Highways typically contribute a significant portion of the night lights observed from space (Oliver, n.d.). Therefore, it is important to avoid mistakenly identifying areas with reduced traffic as power outages. To streamline data acquisition, a shapefile of all Texas highways was downloaded from [Geofabrik](https://download.geofabrik.de/), rather than using the larger OpenStreetMap dataset.

## Contributors

This repository is maintained by Vedika Shirtekar as part of the Master of Environmental Data Science program at UC Santa Barbara. Thanks to the Bren School of Environmental Science and Management for facilitating data access and documentation.

## References

Bureau, U. C. (n.d.). American community survey (ACS). Census.Gov. Retrieved November 10, 2025, from <https://www.census.gov/programs-surveys/acs>

Download openStreetMap for openStreetMap data extracts. (n.d.). Geofabrik Download Server. Retrieved November 10, 2025, from <https://download.geofabrik.de/>

Home. (n.d.). LAADS DAAC. Retrieved November 10, 2025, from <https://ladsweb.modaps.eosdis.nasa.gov/>

Houston, TX. (n.d.). Data USA. Retrieved November 10, 2025, from <https://datausa.io/profile/geo/houston-tx>

Oliver, R. (n.d.). Homework assignment 3. Retrieved November 10, 2025, from <https://eds-223-geospatial.github.io/assignments/HW3.html#rubric-specifications>

Zhou, R. Z., Hu, Y., Zou, L., Cai, H., & Zhou, B. (2023). Understanding the disparate impacts of the 2021 texas winter storm and power outages through mobile phone location data and nighttime light images. Elsevier BV. <https://doi.org/10.2139/ssrn.4631641>
