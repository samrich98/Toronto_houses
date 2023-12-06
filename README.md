# How Temporal and Geographical Factors Can Improve a Sale Price Prediction Model in Toronto
This repository shows an analysis of the Toronto housing market from 2014 to 2023 including the influence of financial, crime, and local factors. A model is created using this analysis to compare how those factors influence the final sale price.

# The Notebooks:
The notebooks are listed 1-9, the order in which they should be run. Notebooks 1 and 2 involved scraping and cleaning the housing data. Notebooks 3-5 contain the code for combining the additional features such as nearby infrastructure (Notebook 3), nearby amenities and features (Notebook 4), and finally the main notebook (Notebook 5). The main notebook combines the previous notebooks, adding financial and crime features. It also exports the test and train CSV files for the model. Notebook 6 contains all the code required to train and run the model. The final 3 notebooks contain different types of visualizations.

# The Data:
All the data used in this project, other than the housing data, is pulled from various CSV files. They are as follows:
Green Spaces - 4326.csv -> CSV of types and locations of green spaces across Toronto (Source: https://ckan0.cf.opendata.inter.prod-toronto.ca/el/dataset/green-spaces)
INDINF_CPI (1).csv -> Canadian Inflation Data (Source: https://www.bankofcanada.ca/rates/indicators/capacity-and-inflation-pressures/inflation/)
Major_Crime_Indicators_Open_Data.csv -> Toronto Major Crime Data (Source: https://data.torontopolice.on.ca/pages/major-crime-indicators)
School locations-all types data - 4326.csv -> Toronto School locations (Source: https://ckan0.cf.opendata.inter.prod-toronto.ca/tr/dataset/school-locations-all-types)
Toronto-population-2023-11-20.csv -> Toronto Population Data (Source: https://www.macrotrends.net/cities/20402/toronto/population)
address-points-4326.csv -> Addresses in Toronto (Source: https://ckan0.cf.opendata.inter.prod-toronto.ca/ne/dataset/address-points-municipal-toronto-one-address-repository/resource/64d4e54b-738f-4cd9-a9e7-8050fac8a52f)
infrastructure_childcare.csv -> Ontario Childcare Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
infrastructure_communities.csv -> Ontario Communities Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
infrastructure_education.csv -> Ontario Education Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
infrastructure_healthcare.csv -> Ontario Healthcare Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
infrastructure_recreation.csv -> Ontario Recreation Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
infrastructure_roadsandbridges.csv -> Ontario Roads Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
infrastructure_transit.csv -> Ontario Transit Infrastructure Data (Source: https://data.ontario.ca/dataset/ontario-builds-key-infrastructure-projects)
interest rates.csv -> Toronto Morgage Interest Rates (Source: https://wowa.ca/canada-mortgage-rates-history)
unemployment rate.csv -> Ontario Unemployment Rates (Source: https://ycharts.com/indicators/ontario_unemployment_rate)

# Checkpoints:
The following files are included in the Repository so the full code does not have to be run. Creating and processing some of this data can take hours. Note that due to a 25MB file upload limit size on GitHub, some files have been truncated. Running 
Houses_Infrastructure_10km.csv -> Infrastructure within 10 km of a house. Create by changing Radius of influence to 10000
Houses_Infrastructure_1km.csv -> Infrastructure within 10 km of a house. Create by changing the Radius of influence to 1000
Houses_Infrastructure_2km.csv -> Infrastructure within 10 km of a house. Create by changing the Radius of influence to 2000
Houses_Infrastructure_3km.csv -> Infrastructure within 10 km of a house. Create by changing the Radius of influence to 3000
Houses_Infrastructure_4km.csv -> Infrastructure within 10 km of a house. Create by changing the Radius of influence to 4000
Houses_Infrastructure_5km.csv -> Infrastructure within 10 km of a house. Create by changing the Radius of influence to 5000
Houses_Infrastructure_7km.csv -> Infrastructure within 10 km of a house. Create by changing the Radius of influence to 7000
houses_data.csv -> cleaned housing data with only 50 features
houses_data_final.csv -> checkpoint created midway through the main notebook. Includes engineered house features
nearby_features.csv -> output of the nearby features notebook for merging with the main data frame in the main notebook
save-0-10,000.csv -> example of first 10,000 data points scraped from Zolo.ca
this_is_the_completed_csv!.csv -> final data set for visualizations
test.csv -> chronologically the last 20% of data. Used to test the model.
train.csv -> chronologically the first 80% of data. Used to train the model.

# Shapefiles:
The following shapefiles were used to in this repository:
subway_stations.dbf<br />
subway_stations.prj
subway_stations.sbn
subway_stations.sbx
subway_stations.shp
subway_stations.shp.xml
subway_stations.shx
toronto_neighbourhoods.cpg
toronto_neighbourhoods.dbf
toronto_neighbourhoods.prj
toronto_neighbourhoods.shp
toronto_neighbourhoods.shx
