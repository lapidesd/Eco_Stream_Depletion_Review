# Environmental flows approaches to stream depletion management: supporting code and data

Reductions in streamflow can impact aquatic ecosystems in streams. Here, we use an environmental flows approach to explore how streamflow depletion from groundwater pumping impacts aspects of the hydrograph and thermograph that are important for aquatic ecosystems. This repository contains:
* **metric_impacts**: a directory containing jupyter notebooks to calculate impacts in a suite of metrics for streamflow and stream temperature respectively.
    * **flow_metric_change.ipynb**: Jupyter notebook to calculate impacted hydrographs for each hydrograph in a set of 34 Wisconsin hydrographs <40 cfs from USGS historical streamflow data ([https://waterdata.usgs.gov/nwis/sw](https://waterdata.usgs.gov/nwis/sw)). The differences between impacted and unimpacted hydrographs are measured using a suite of metrics described in Lapides et al. (2021).
    * **temp_metric_change.ipynb**: Jupyter notebook to calculate unimpacted and impacted thermographs for each hydrograph in a set of 34 Wisconsin hydrographs <40 cfs using an end-member mixing model with two reservoirs (groundwater and surface water). The differences between impacted and unimpacted thermographs are measured using a suite of metrics described in Lapides et al. (2021).
    * **metric_test_example.ipynb**: Jupyter notebook to demonstrate how the choice of metric can impact management decisions, as described in Lapides et al. (2021).
* **longterm_site_data_rev1**: a directory containing timeseries of streamflow depletion in m3/d for a pumping schedule simulated using the Glover Equation (Glover, 1954) as implemented in [StreamDepletr](https://cran.r-project.org/web/packages/streamDepletr/index.html). The simulated wells are 1,000m from the stream with  hydraulic conductivity of K = 1 m/d, aquifer thickness of b = 100 m, and specific yield of Sy = 0.2. The pump rate is given in the file name for each file in m3/d.
* **streamflow_data**: hydrograph data for each of 135 Wisconsin streams from USGS historical records ([https://waterdata.usgs.gov/nwis/sw](https://waterdata.usgs.gov/nwis/sw)). Files are named by USGS site number. Also contains air temperature data for Madison, WI (temp_data_noaa.csv) from NOAA climate records ([https://www.ncdc.noaa.gov/cdo-web/](https://www.ncdc.noaa.gov/cdo-web/)).


# References:

Glover, Robert E., and Glenn G. Balmer. "River depletion resulting from pumping a well near a river." Eos, Transactions American Geophysical Union 35.3 (1954): 468-470.

Lapides D, Maitland B, Zipper S, Latzka A, Pruitt A, Greve R (2021). Advancing environmental flow approaches to streamflow depletion management.
