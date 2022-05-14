# New York City Emissions Intensity Map
##### Notebook by [Mohamad Razkenari](https://www.razkenari.com)

<img src="https://www.urbangreencouncil.org/sites/default/files/landing_page_image.jpg"/>

## Introduction

To reduce carbon emissions from buildings, the City of New York enacted [Local Law 97 (LL97)](https://www1.nyc.gov/site/sustainablebuildings/ll97/local-law-97.page) in 2019 as a part of the Climate Mobilization Act. This law places carbon caps on most buildings larger than 25,000 square feet—roughly 50,000 residential and commercial properties across NYC. These caps start in 2024 and will become more stringent over time, eventually reducing emissions 80 percent by 2050. This project uses building energy consumption and building characteristics data to calculate the emissions intensity, and compare it with the emissions limit according to building end use classification. Then, maximum penalty for non-compliance is calculated.

Here’s what you need to know about LL97

* Applies to all buildings in NYC greater than 25000 square feet; applicable for approximately 60% residential and 40% commercial buildings
* Penalties for non-compliance; maximum penalty is calculated based on the difference between a building’s annual emissions limit and its actual emissions multiplied by 268
* A building’s annual emissions limit equals its emissions intensity limit multiplied by its gross floor area
* Many buildings are significantly above emissions limits and will require comprehensive retrofits or potentially face millions of dollars in penalties
* There are two increasingly stringent phases of limits; first phase takes effect in 2024 and the second occurring in 2030
* Emissions intensity limits (metric tons of CO2e per square foot) are set based on 10 building categories defined by Building Code occupancy groups
* Renewable energy credits and/or emissions offsets can be used to comply with the caps

>**Project Objective**: Calculate Emissions Intensity for buildings in New York City, and assess their compliance with Local Law 97.

## Required libraries
This notebook uses several Python packages that come standard with the Anaconda Python distribution. The primary libraries that we'll be using are:

* **NumPy**: Provides a fast numerical array structure and helper functions.
* **Pandas**: Provides a DataFrame structure to store data in memory and work with it easily and efficiently.
* **Scikit-learn**: The essential Machine Learning package in Python.
* **Matplotlib**: Basic plotting library in Python; most other Python plotting libraries are built on top of it.
* **Seaborn**: Advanced statistical plotting library.
* **GeoPandas**: GeoPandas is an open source project to make working with geospatial data in python easier.
* **ArcGIS**: Advanced library to convert and manage geographic data, automate spatial workflows, perform advanced spatial analytics.
* **Sodapy**: API for getting NYC data.
* **folium**: A library to create several types of Leaflet maps

## Required Datasets

**To calculate Emissions Intensity:** Emissions intensity is the total global warming potential per square foot per year, measured in kg CO2e/m2/a
* [Energy use benchmarking data](https://data.cityofnewyork.us/Environment/Energy-and-Water-Data-Disclosure-for-Local-Law-84-/usc3-8zwd) (anual energy consumption, including natural gas, electricity, and district steam - NYC Open Data, LL84)    
* [Building footprint data](https://data.cityofnewyork.us/Housing-Development/Building-Footprints/nqwf-w8eh) (available in NYC Open Data)
* [Building 3D models](https://www1.nyc.gov/site/doitt/initiatives/3d-building.page) (available in NYC Open Data)

**To identify Emissions Target:** Emissions limit are specifed in the LL97 based on the building classification for 2024 and 2030. 
* [Building Use and Characteristics](https://www1.nyc.gov/site/planning/data-maps/open-data/bytes-archive.page?sorts[year]=0) (available in NYC Open Data)

## [Live Dashboard](https://www.razkenari.com/NYC-EIM)
