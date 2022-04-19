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

** Featureset Exploration **

* **age**: continuous. 
* **workclass**: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked. 
* **education**: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool. 
* **education-num**: continuous. 
* **marital-status**: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse. 
* **occupation**: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces. 
* **relationship**: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried. 
* **race**: Black, White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other. 
* **sex**: Female, Male. 
* **capital-gain**: continuous. 
* **capital-loss**: continuous. 
* **hours-per-week**: continuous. 
* **native-country**: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.
