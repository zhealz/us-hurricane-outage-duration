# Data sources

Every input is public. The tables in `us_flood_outage/` are county-level summaries derived from them; no original file is redistributed here.

| Input | Used for | Access in the notebooks | Terms | Citation |
| --- | --- | --- | --- | --- |
| EAGLE-I recorded electricity outages | Outage labels (Steps 1b, 2c, 2d) | Yearly files on figshare (file ids are in the notebooks); the 2014–2022 record is [doi:10.6084/m9.figshare.24237376](https://doi.org/10.6084/m9.figshare.24237376), and the 2024 file used for Beryl and Helene was published later | See the figshare record; the data descriptor is CC BY 4.0 | Brelsford, C. et al. (2024). A dataset of recorded electricity outages by United States county 2014–2022. *Scientific Data* 11, 271. [doi:10.1038/s41597-024-03095-5](https://doi.org/10.1038/s41597-024-03095-5) |
| NHC Tropical Cyclone Reports | Landfall times and places | [nhc.noaa.gov/data/tcr](https://www.nhc.noaa.gov/data/tcr/) | U.S. Government work | NOAA National Hurricane Center |
| IBTrACS v04r01, North Atlantic | Storm tracks, wind radii | NOAA NCEI | U.S. Government work | Knapp, K. R. et al. (2010). The International Best Track Archive for Climate Stewardship (IBTrACS). *Bulletin of the American Meteorological Society* 91, 363–376 |
| NOAA Real-Time Mesoscale Analysis (RTMA) | Gusts and wind speed | Earth Engine `NOAA/NWS/RTMA` | U.S. Government work | NOAA National Weather Service |
| PRISM daily precipitation | Rainfall | Earth Engine `OREGONSTATE/PRISM/ANd` | No restriction on use or distribution; attribution requested | PRISM Climate Group, Oregon State University; Daly, C. et al. (2008). *International Journal of Climatology* 28, 2031–2064 |
| NLCD 2019 | Land cover, impervious surface | Earth Engine `USGS/NLCD_RELEASES/2019_REL/NLCD` | U.S. Government work | U.S. Geological Survey, National Land Cover Database |
| SRTM 1 arc-second | Elevation, low-lying land | Earth Engine `USGS/SRTMGL1_003` | Public | NASA / USGS |
| American Community Survey, 5-year estimates | Population, housing, income | Census API (key required) | U.S. Government work | U.S. Census Bureau |
| Census county population estimates | Customer totals per county | census.gov | U.S. Government work | U.S. Census Bureau |
| HHS emPOWER | Users of electricity-dependent medical equipment | HHS emPOWER REST service | Public | U.S. Department of Health and Human Services |
| Copernicus Sentinel-1 GRD | Flood extent by change detection | Earth Engine `COPERNICUS/S1_GRD` | Copernicus open data terms | Contains modified Copernicus Sentinel data |
| MERIT Hydro v1.0.1 | Height above the nearest drainage | Earth Engine `MERIT/Hydro/v1_0_1` | CC BY-NC 4.0 or ODbL 1.0 | Yamazaki, D. et al. (2019). MERIT Hydro: a high-resolution global hydrography map based on latest topography datasets. *Water Resources Research* 55, 5053–5073 |
| JRC Global Surface Water v1.4 | Permanent water mask | Earth Engine `JRC/GSW1_4/GlobalSurfaceWater` | Free with attribution | Pekel, J.-F. et al. (2016). High-resolution mapping of global surface water and its long-term changes. *Nature* 540, 418–422 |
| GHSL built-up surface (P2023A) | Built-up mask | Earth Engine `JRC/GHSL/P2023A/GHS_BUILT_S` | Free with attribution | European Commission, Joint Research Centre, Global Human Settlement Layer |
| NASA Black Marble VNP46A2 | Night lights (independent check) | Earth Engine `NASA/VIIRS/002/VNP46A2` | NASA open data | Román, M. O. et al. (2018). NASA's Black Marble nighttime lights product suite. *Remote Sensing of Environment* 210, 113–143 |
| AlphaEarth Foundations Satellite Embedding V1, annual | County embeddings | Earth Engine `GOOGLE/SATELLITE_EMBEDDING/V1/ANNUAL` | CC BY 4.0 | Brown, C. F. et al. (2025). AlphaEarth Foundations: an embedding field model for accurate and efficient global mapping from sparse label data. [arXiv:2507.22291](https://doi.org/10.48550/arXiv.2507.22291) |
| TIGER 2018 county boundaries | County geometry for zonal statistics | Earth Engine `TIGER/2018/Counties` | U.S. Government work | U.S. Census Bureau |
| County outlines for the map | Figure 1 | [plotly/datasets](https://github.com/plotly/datasets), `geojson-counties-fips.json` | Derived from U.S. Census Bureau cartographic boundary files | U.S. Census Bureau |

Required attribution: The AlphaEarth Foundations Satellite Embedding dataset is produced by Google and Google DeepMind.

Step 1b also reads the Global Flood Database (`GLOBAL_FLOOD_DB/MODIS_EVENTS/V1`) for a visual comparison; nothing derived from it is used later.
