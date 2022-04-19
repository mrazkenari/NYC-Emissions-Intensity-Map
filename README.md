# New York City Emissions Intensity Map
##### Notebook by [Mohamad Razkenari](https://www.razkenari.com)

<img src="https://www.urbangreencouncil.org/sites/default/files/landing_page_image.jpg"/>

## Introduction
In the time it took you to read this sentence, terabytes of data have been collectively generated across the world — more data than any of us could ever hope to process, much less make sense of, on the machines we're using to read this notebook.

<img src="https://www.circuitmeter.com/wp-content/uploads/2020/02/image-industryArticles_NYC-LL97.jpg" width=50% />


>**Note:** Please specify.

Here’s what you need to know

* Applies to all buildings in NYC greater than 25000 square feet; applicable for approximately 60% residential and 40% commercial buildings
* Penalties for non-compliance; maximum penalty is calculated based on the difference between a building’s annual emissions limit and its actual emissions multiplied by 268
* A building’s annual emissions limit equals its emissions intensity limit multiplied by its gross floor area
* Many buildings are significantly above emissions limits and will require comprehensive retrofits or potentially face millions of dollars in penalties
* There are two increasingly stringent phases of limits; first phase takes effect in 2024 and the second occurring in 2030
* Emissions intensity limits (metric tons of CO2e per square foot) are set based on 10 building categories defined by Building Code occupancy groups
* Renewable energy credits and/or emissions offsets can be used to comply with the caps

## Required Datasets

**Step 1 - Calculate Emissions Intensity**: total global warming potential per square foot per year, neasured in kg CO2e/m2/a
* Energy Consumption per year
 * Natural Gas
 * Electricity
 * District Steam
* Building Floor area 

**Step 2 - Identify Emissions Target**: Based on building classification, as specified by the Local Law 97
* Building Occupancy Classification
* Global Warming Potential per unit of energy

**Data Sources:**
* **Energy use benchmarking data** (required by LL84) [LINK](https://data.cityofnewyork.us/Environment/Local-Law-84-2021-Monthly-Data-for-Calendar-Year-2/in83-58q5) 
* **Building footprint data** [LINK](https://data.cityofnewyork.us/Housing-Development/Building-Footprints/nqwf-w8eh)
* **Building 3D models** [LINK](https://www1.nyc.gov/site/doitt/initiatives/3d-building.page)
* **Building Use and Characteristics** [LINK](https://www1.nyc.gov/site/planning/data-maps/open-data/bytes-archive.page?sorts[year]=0)