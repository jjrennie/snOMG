# #snOMG
## Written By Jared Rennie (@jjrennie)

Have you wondered how much snow occurred on a certain date (or range of dates?) This notebook will help you answer that question. We will be using data from <a href='http://www.ncei.noaa.gov' target='_blank'> NOAA's National Centers of Environmental Information</a>, specifically the Global Historical Climatology Network - Daily Dataset: 

- GHCNd Info: https://www.ncei.noaa.gov/products/global-historical-climatology-network-daily
- GHCNd AWS Location: https://registry.opendata.aws/noaa-ghcn/

In order to understand gridded vs observed, we will also look at data from the National Gridded Snowfall Analysis run by the <a href='http://www.nohrsc.noaa.gov' target='_blank'> National Operational Hydrologic Remote Sensing Center (NOHRSC) </a>
- NOHRSC Info: https://www.nohrsc.noaa.gov/snowfall_v2/
- NOHRSC Data: https://www.nohrsc.noaa.gov/snowfall_v2/data

In addition to answering these questions, you will learn how to get data from the cloud (and elsewhere) and plot it, without actually reading in the entire dataset!

## What You Need
First off, the entire codebase works in Python 3. In addition to base Python, you will need the following packages installed: 
- numpy, pandas, and xarray (to slice annd dice the data)
- scipy, geopandas, and rioxarray (to read in some shapefiles and do GIS calculations)
- pyarrow or fastparquet (for the parquet data ingest)
- matplotlib and cartopy (to plot)
  
The "easiest" way is to install these is by installing <a href='https://www.anaconda.com' target="_blank">anaconda</a>, and then applying <a href='https://conda-forge.org/' target="_blank">conda-forge</a>. Afterward, then you can install the above packages. 