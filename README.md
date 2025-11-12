# Lights Out in Houston: Mapping the Effects of Winter Storm Uri

## Description

Winter Storm Uri was a powerful and catastrophic winter storm that devastated several communities in Texas during February 13-17 2021. The state was unprepared for a significant loss of power; power plants and grids were not prepared to handle freezing temperatures coupled with increased electricity usage to heat homes (Zhou et al., 2024). Nearly 246 people perished, 4.5 million homes lost power, and costed the state about \$195 million in damages (Zhou et al., 2024). As such, Winter Storm Uri is listed as the costliest and one of the deadliest natural disasters in Texas history.

Harris County was heavily impacted by the storm. The City of Houston, the most populous city in Harris County, has a population of 2,333,346 people as of 2024 (City of Houston, .

The purpose of this assignment is to assess the extent to which houses and census tracts in Houston lost power during Winter Storm Uri. The analysis utilizes spatial manipulation between raster and vector types to identify homes in Houston that experienced a blackout, as well as an assessment of median income for census tracts affected by the blackout based on socioeconomic data. The following research question was referenced to guide the analysis:

**To what extent were homes and census tracts in Houston impacted by the power outage caused by Winter Storm Uri?**

## Repository Structure

This repository contains:

## Data Description and Access

VIIRS data was obtained from NASA Worldview platform is an open source database to

Use NASA’s Worldview to explore the data around the day of the storm. There are several days with too much cloud cover to be useful, but 2021-02-07 and 2021-02-16 provide two clear, contrasting images to visualize the extent of the power outage in Texas.

VIIRS data is distributed through NASA’s [Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center (LAADS DAAC)](https://ladsweb.modaps.eosdis.nasa.gov/). Many NASA Earth data products are distributed in 10x10 degree tiles in sinusoidal equal-area projection. Tiles are identified by their horizontal and vertical position in the grid. Houston lies on the border of tiles h08v05 and h08v06. We therefore need to download two tiles per date.

As you’re learning in EDS 220, accessing, downloading, and preparing remote sensing data is a skill in it’s own right! To prevent this assignment from being a large data wrangling challenge, we have downloaded and prepped the following files for you to work with, stored in the `VNP46A1` folder.

## Authors and Additional Contributors

## References
