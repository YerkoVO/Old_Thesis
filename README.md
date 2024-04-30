# Datasets for Thesis: Impact on the Supply Chain of the Declaration to Triple Global Nuclear Energy Production by 2050

## **Description**:

This repository contains the datasets used in the research for the thesis titled "Impact on the Supply Chain of the Declaration to Triple Global Nuclear Energy Production by 2050". The provided data here are crucial for analyzing and assessing the anticipated effects of nuclear expansion on the global supply chain, particularly in the context of forecasting the triple global energy production by 2050 and examining the continental contributions to world electricity production.

## **Repository Structure**:

**- datasets:** Contains the original datasets used as input for models and analysis.

**- scripts:** Contains the scripts and codes used for data analysis and result generation.

**- results:** Contains the results of the analyses performed on the datasets.

**- documentation:** Contains any relevant documentation related to the datasets and analyses conducted.

## **Available Datasets**:

**World_electricity.csv:** Contains historical data on global electricity production, broken down by energy type. This data is crucial for understanding energy demand and its impact on the supply chain. It is also used to compare forecasted world electricity production by 2050 with actual data and analyze the percentage contribution of each continent to global electricity production.

**Owid.csv:** This dataset is a collection of key metrics maintained by [OWID](https://ourworldindata.org/energy), it is necessary to mention that the data used from this dataset for the development of the thesis comes from [IAEA](https://pris.iaea.org/pris/). Specific data such as nuclear power generation and nuclear electricity were extracted, retaining all countries and dates in the dataset for further analysis. This dataset is used to project the increase in global electricity production, as well as to project the tripled global nuclear power production by 2050 and assess the percentage contributions to total electricity generation by continent.

## **Available Scripts**:

**World_Nuclear_Electricity_Production.ipynb**: This notebook analyzes and visualizes the production of nuclear electricity by region over time, using data extracted from Our World in Data (Owid). It starts by filtering country data to remove entries not relevant to actual countries (e.g., those labeled with entities like Shift or Ember). It then categorizes countries into regions such as Africa, Asia, and North America, among others. Using these regions, the notebook plots the historical nuclear electricity production from 1985 up to the most recent data point, illustrating trends and developments over the years.

**World_Electricity_Production_bySource.ipynb**: This notebook visualizes global electricity production from various energy sources over time. It processes data on energy sources including coal, oil, gas, nuclear, hydro, wind, solar, and biofuels. By employing a stacked plot, it illustrates the relative contributions of each energy source to total electricity production from 1985 to the present. The plot highlights trends in energy usage and transitions between different energy sources. Additionally, the notebook quantifies nuclear electricity production for the year 2021, summarizing the total production from this source.

**World_electricity_forecast.ipynb**: This notebook integrates regional nuclear electricity forecasts with global data to update world electricity forecasts. It processes COP28-specific predictions and global nuclear electricity production data by mapping countries to their respective regions and adjusting the global forecasts based on regional data from COP28. The final output is an updated global forecast, saved to a CSV file, which aims to refine global nuclear electricity production estimates by incorporating the latest regional forecasts.

**World_electricity_production.ipynb**: This notebook explores historical data and future projections of global electricity production. Using data sourced from Our World in Data, it focuses on worldwide electricity generation statistics, beginning with a plot of historical data from 1985. This historical analysis sets the stage for integrating forecast data, which predicts electricity generation up to the year 2050. The notebook merges historical data with forecasted data to present a continuous timeline, which is visualized in a detailed line plot that highlights both the historical records and future projections. Specific forecast values for the years 2030 and 2050 are extracted and displayed, providing insights into expected trends in global electricity production.

**Nuclear_Electricity_Cop28_Forecasts.ipynb**: This notebook is dedicated to projecting future nuclear electricity production for a select group of countries involved in the COP28 framework. It starts by loading historical electricity data and identifies a specific list of countries participating in COP28. For each country, it calculates the last recorded value of nuclear electricity production. The notebook then sets a target to triple this value by the year 2050. Using a compound annual growth rate, it forecasts nuclear electricity production annually from 2023 to 2050. The final forecasts are stored in a DataFrame, which is then exported to a CSV file. This analysis helps to visualize and understand the growth trajectory of nuclear energy in response to COP28 commitments.

**Nuclear_Electricity_World_Forecasts.ipynb**: This notebook focuses on forecasting global nuclear electricity production using advanced time series analysis methods. It starts by importing global electricity data, which it then processes to distinguish between COP28 countries and others, grouping the latter into regional categories. The notebook employs statistical tests to ensure the data's suitability for time series forecasting and utilizes the SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors) model for this purpose.
Key steps in the analysis include identifying the best model parameters through AIC minimization, fitting the model to historical data, and then forecasting nuclear electricity production up to the year 2050. It provides a detailed forecast including confidence intervals, emphasizing the statistical rigor of the process. The forecasts are saved to a CSV file, aiming to provide actionable insights on future trends in global nuclear electricity generation.



