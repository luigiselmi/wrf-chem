WRF-CHEM
========
This repository is used to set up the processing pipeline to transform datasets from the Copernicus services CAMS (air quality) and C3S (meteorology) to a format that can be used as input to [WRF-CHEM](https://www2.acom.ucar.edu/wrf-chem) for the initialization of the model. The procedure for the download and processment is described in the [ECWMWF knowledge base](https://confluence.ecmwf.int/pages/viewpage.action?pageId=174865233). The main steps are

1. Download the meteorological data (ERA5 Reanalysis) from Copernicus C3S
2. Download the air quality data from CAMS
3. If the datasets are in the GRIB format they must be transformed in NetCDF
4. The CAMS data must be interpolated to match the WRF grid

Once all the steps have been performed we can run WRF-CHEM.