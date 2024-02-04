# PROJECT Description:

Organization: Uniper Trading Canada Ltd

Project Title: How do weather conditions and natural gas production levels in Alberta impact natural gas
prices?

Problem Statement: Weather conditions have a large impact on natural gas prices through their effect
on heating fuel consumption and electricity generation. A good understanding of the impact of weather
on gas prices is needed to inform trading strategies.

Objective: Determine if there is a correlation between weather patterns (like cold snaps or heat waves)
and natural gas prices, analyze the relationship between production levels and prices. Forecast
Scenarios. This is an El Nino year - outline some extraordinary weather scenarios accompanied by some
possible expected prices.

Data: There are numerous public datasets that may be useful in the analysis. Some examples are
provided here - feel free to look for others.

- Alberta Natural Gas Prices: The Alberta government provides historical natural gas reference
prices from 1994 to the present. These prices are available monthly by year and can be a vital
source for analyzing price trends. Access the data at: https://www.alberta.ca/alberta-natural-gas-reference-price

- Alberta Historical Weather Data: The Alberta Climate Information Service (ACIS) offers an online
interactive Historical Weather Data Viewer. This tool allows users to view daily meteorological
records for numerous points across the province dating back to 1961. The data can be viewed as
tables or graphs and downloaded for further analysis. Access the data at:
https://www.alberta.ca/acis-find-historic-climate-data

- Alberta Natural Gas Production Data: The Alberta Energy Regulator provides detailed
information on the average daily production of marketable natural gas in Alberta. The data
includes historical trends and forecasts for future production. The data is available in an XLSX
format, which is suitable for analysis. Access the data at: https://www.aer.ca/providing-information/data-and-reports/statistical-reports/st98

## Data Analysis Outline

### 1. Data Preparation and Cleaning
1. Use Python CSV Scraper code to combine all 50 US weather data files into one file: combined_us_weather_data (deleted "Station code" column)
2. Use Python CSV Scraper code to combine all 19 Canada weather data files into one file: combined_ca_weather_data (deleted "Longitude (x)", "Latitude (y)", "Climate ID", "Data Quality", "Max Temp Flag", "Min Temp Flag", "Mean Temp Flag", "Heat Deg Days Flag", "Cool Deg Days Flag", and other "flag" columns)
3. In "alberta_weather" file, deleted: "Air_Temp._Min._(°C)_interpolation_flags", and other "flags" columns"

### 2. Exploratory Data Analysis
* Summary statistics overview (mean, median)
* Weather pattern analysis (categorize temperature, extraordinary weather conditions, etc)
* Trend detection (seasonal trends or pattern)

### 3. Correlation Analysis
* Scatter plots
* Heatmaps
* Linear regression

### 4. Forecasting
* ARIMA
* Mchine learning
* El Niño impact