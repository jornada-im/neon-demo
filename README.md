# neon-demo: Accessing data from the Jornada NEON site

This respository contains notes and demonstrations on using data from the National Ecological Observatory Network, or NEON. There is a NEON site, named "JORN", located in the Jornada Basin near the IBP exclosure. For more information on JORN, other sites, or NEON in general, visit <https://www.neonscience.org>.

Much of the content in the included demos came from the NEON data workshop held at UTEP and NMSU in November 2019. Details can be found at the [workshop page](https://www.neonscience.org/resources/workshops/explore-neon-workshop-utep-nmsu-2019) (click "Workshop Materials" for links to materials).

## Getting started

There are 47 terrestrial and 34 freshwater aquatic NEON field sites, arranged in 20 ecological domains across the continental U.S. The terrestrial NEON site at the Jornada Basin ([JORN](https://www.neonscience.org/field-sites/field-sites-map/JORN)) is located in the Desert Southwest domain (D14) and is classified as one of NEON's "relocatable" sites. The cover is mainly black-grama grassland, but there are yucca and mesquite mixed in.

There are many data products (or datasets) available at NEON sites, and measurement methods and design are standardized across all terrestrial or aquatic sites. NEON additionally classifies the data products based on how they were collected. Observation systems (OS) datasets were collected by human observers, instrumented systems (IS) datasets were collected by sensor networks, and airborn observing platform (AOP) datasets were collected by NEON's airborn sensor payload.  All data products have different QAQC levels that are [described on the NEON website](https://www.neonscience.org/data/about-data/data-processing-publication).

**Important NEON website functionality**

* The [data product catalog](https://data.neonscience.org/data-product-catalog) lists the different data products that are available across NEON sites. The list, which is long, can be filtered by observation class and QA level.
* The [field site map](https://www.neonscience.org/field-sites/field-sites-map) allows acces to further information about NEON sites through a map interface.
* From the [data portal](http://data.neonscience.org/static/browse.html) data files can be downloaded manually as zip or other archive formats depending on the data product (This portal is in development, but should become the main portal soon).
* Documentation files are in the [documents library](https://data.neonscience.org/documents). They are not particularly easy to search here, but luckily, if you find data products on the data portal or download them as archives, the correct documentation files should be included as ancillary links or files.

**R tools for accessing NEON data**

For R users NEON has created several R packages that make downloading and importing NEON data into the R environment easy. The list of useful utilities and commands to install them are below:

* neonUtilities: `install.packages("neonUtilities")`; to access NEON data specific functions
* raster: `install.packages("raster")`; to work with raster files in R
* rhdf5: `install.packages("BiocManager"), BiocManager::install("rhdf5")`; to work with HDF5 files in R
* devtools: `install.packages("devtools")`; required to install using the install_github() function.
* geoNEON: `install_github("NEONScience/NEON-geolocation/geoNEON”)`; to get specific location data for NEON data and samples. You must have devtools installed and running ( library(devtools)) prior to installing with install_github(). For further directions, see the start of the Use the neonUtilities Package to Access NEON Data tutorial.

## Useful general NEON tutorials

NEON has a number of tutorials that help users learn how to access and explore data products. These are a good way to gain familiarity with the R tools NEON provides, and illustrate some of the advantages and pitfalls of using NEON data.

1. [Download and explore NEON data](https://www.neonscience.org/download-explore-neon-data)
2. [Detailed neonUtilities tutorial](https://www.neonscience.org/neonDataStackR)
3. [Access and work with NEON Geolocation Data](https://www.neonscience.org/neon-spatial-data-basics)
4. [Linking ground observations and remote sensing (AOP) data](https://www.neonscience.org/tree-heights-veg-structure-chm)

A complete list of NEON tutorials can be found [here](https://www.neonscience.org/resources/data-tutorials).

## Exploring Jornada (and cross-site) NEON data

These are based on the general NEON tutorials above, but specifically use JORN data and address Jornada research themes. The links are to Jupyter notebooks on GitHub, which should render in most browsers.

1. to come...
2. [Exploring NEON eddy covariance data at JORN](eddyflux_demo_JORN.ipynb)
