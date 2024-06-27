Choose the Right Vehicle for You: A Data-Driven Exploration of the U.S. Gas-Powered Car Market (2014-2020) 
 
![dashboard1](https://github.com/Berat-rex/Cars_Capstone/assets/156152859/dcf8eddb-5d18-4eab-9b07-7d042fd90ae4)

This Tableau dashboard empowers consumers to make informed car buying decisions by providing data-driven insights into the fuel efficiency, cost, emissions, and size of various vehicle brands from 2014 to 2020. It's designed to simplify the complex process of choosing the right car by allowing users to filter and compare vehicles based on their individual priorities.
---
Table of Contents:
- Introduction
- Key Questions
- Data Sources
- Methodology
- Key Findings
- Limitations
- Visualizations
- Technologies
- Future Work

---
Introduction:

This project delves into the heart of the American car market, focusing on gasoline-powered vehicles from 2014 to 2020. By combining data from the U.S. Department of Energy and real-world used car listings, we uncover trends and patterns that reveal which cars excel in fuel efficiency, cost-effectiveness, environmental impact, size, and more. Whether you're a budget-conscious commuter, an eco-conscious driver, or a performance enthusiast, this dashboard provides the insights you need to choose the right vehicle for you.

---
Key Questions:

1.	Which car brands and vehicle classes consistently offer the highest miles per gallon (MPG) between 2014 and 2020?
2.	How has the average fuel efficiency of different car brands evolved over the years? Are there any noticeable trends or improvements?
3.	Which specific car brands stand out as the most fuel-efficient within their respective vehicle classes and price ranges?
4.	Is there a relationship between the number of cylinders and fuel efficiency?
5.	How does the average price vary across different car brands and vehicle classes?
6.	Which car brands offer the most cost savings in terms of fuel expenses over a five-year period?
7.	What is the relationship between fuel efficiency and purchase price? 
8.	How does the price of a vehicle vary depending on the state?
9.	Which states have the highest and lowest average vehicle prices?
10.	Are there significant differences in CO2 emissions between cars with different number of cylinders?
11.	Which car sizes have the lowest CO2 emissions, and how have emissions trends changed over time (2014-2020)?
12.	Do cars with higher fuel economy scores also tend to have higher greenhouse gas scores?

---
Data Sources:

1. Fuel Economy Data:  Sourced from the U.S. Department of Energy's Fuel Economy website (https://www.fueleconomy.gov/feg/ws/index.shtml#vehicle),
this dataset provides detailed information on the fuel efficiency of various vehicles, including city and highway MPG, annual fuel cost estimates, and greenhouse gas ratings.
2. Used Car Price Data:  Sourced from the "Craigslist Cars/Trucks Data" dataset on Kaggle (https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data?select=vehicles.csv),
this dataset offers real-world prices for used cars across different makes, sizes, and years.

---
Methodology:

1. Data Collection:
- Fuel Economy Data: Gathered detailed vehicle information and fuel efficiency data (city, highway, and combined MPG, annual fuel cost estimates, greenhouse gas ratings, emissions, etc.) from the U.S. Department of Energy's Fuel Economy API.
-	Used Car Price Data: Acquired real-world transaction prices for used cars across various makes, sizes, and years from the "Craigslist Cars/Trucks Data" dataset on Kaggle.
2. Data Cleaning and Integration:
-	Python & Pandas: Utilized Python and the Pandas library for extensive data cleaning and preprocessing. This involved:
-	Filtering: Selected gasoline-powered vehicles manufactured between 2014 and 2020.
-	Standardization: Standardized brand names and vehicle classifications for consistency and accuracy.
-	Outlier Handling: Identified and addressed outliers in the price and fuel efficiency data to ensure data integrity.
-	Missing Values: Handled missing values appropriately using imputation or removal techniques.
-	Merging: Merged the fuel economy data with the used car price data using common identifiers (make, size, year), prioritizing the information from the fuel economy dataset in a left join.
-	Category Simplification: Standardized Vehicle Class Size into simplified categories (Sedans, SUVs, Pickup Trucks, Vans) for clearer analysis and visualization.
3.  Tableau Dashboard Development:
-	Tableau Public: Imported the final, cleaned dataset into Tableau Public to create an interactive dashboard.
-	Visualization Design: Designed a variety of visualizations (bar charts, maps, heatmaps, and tables) to answer research questions and highlight key insights.
-	Interactive Features: Incorporated filters, tooltips, and parameters to enable user exploration and customization of the analysis.

---
Key Findings:

1.	Sedans Dominate Fuel Efficiency: Across all years analyzed (2014-2020), sedans consistently achieve the highest average fuel efficiency, making them a compelling choice for cost-conscious and eco-minded drivers.
2.	Value Champions: While car prices have fluctuated over time, certain brands stand out for their long-term value proposition. Honda, Mazda, Lexus, and Hyundai are projected to save consumers money over five years compared to the average vehicle, thanks to their exceptional fuel efficiency.
3.	The Green Advantage: A clear inverse relationship exists between fuel efficiency and CO2 emissions. Smaller, more fuel-efficient vehicles generally have a smaller carbon footprint, contributing to a greener environment.
4.	Price Sensitivity to Location: Prices for the same car model can vary significantly across different U.S. states, highlighting the importance of considering regional factors when making a purchase.
5.	Engine Efficiency and Power based on the number of cylinders: While larger engines typically have more cylinders and offer greater power, this often comes at the expense of fuel efficiency. 

---
Limitations:

1.	Price Data: The price data used in this analysis is based on used car listings and might not accurately reflect the current market value for all vehicles.
2.	External Factors: The analysis does not account for other factors that can influence a car purchase decision, such as safety ratings, reliability, and individual preferences.
3.	*Limited Scope: The dataset only covers gasoline-powered vehicles from 2014-2020 in the U.S. market.

---
Visualizations:

- Explore the interactive dashboard on Tableau Public:  https://public.tableau.com/app/profile/berat.rexhepi
 ![dashboard2](https://github.com/Berat-rex/Cars_Capstone/assets/156152859/c86a6086-8e8a-418a-b68e-eac5fdb76275)
![dashboard3](https://github.com/Berat-rex/Cars_Capstone/assets/156152859/cf63c2b1-94b3-4df5-b0a2-86e544b1dd14)

 ---
Technologies:

- Python: Used for data cleaning, preprocessing, and analysis.
-	Pandas: Python library for data manipulation and analysis.
-	Tableau Public: Used for creating interactive data visualizations.

---
Future Work:

1.	Expand the Dataset: Incorporate data from 2021 onwards to capture the latest trends in the car market and provide users with the most up-to-date information for their car-buying decisions.
2.	Enhance the Analysis:
o	Safety and Reliability: Integrate data on vehicle safety ratings (from sources like NHTSA and IIHS) and reliability scores (from sources like Consumer Reports) to create a more comprehensive picture of each car's value proposition.
o	Additional Factors: Explore the impact of other relevant attributes such as vehicle weight, transmission type, engine power, and technology features on fuel efficiency, cost, and emissions.
o	User Reviews and Ratings: Incorporate consumer feedback through an analysis of online reviews to gauge customer satisfaction and overall perception of different vehicle types.
3.	Develop Predictive Models: Utilize machine learning techniques to build predictive models for:
o	Future Fuel Costs: Estimate the long-term fuel expenses for different car models based on their fuel efficiency and predicted fuel price trends.
o	Vehicle Depreciation: Forecast how the value of different vehicles is expected to change over time, aiding users in making financially wise decisions.
