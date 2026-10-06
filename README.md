# NYC-Philadelphia-Transit-Ridership-Analysis
Data analysis comparing NYC and Philadelphia transit ridership from 2021–2025 using per-capita analysis, t-tests, and linear regression. 

Business Understanding 

- Business Problem: 
Public transportation systems play a critical role in supporting economic activity, commuting efficiency, and urban mobility in major cities. Understanding how the public use different transit modes can provide valuable insight for transportation agencies when making operational and policy decisions.
This project aims to compare public transit ridership between New York City and Philadelphia by analyzing monthly ridership data from their major transit systems. By examining usage patterns across different transportation modes such as buses, subways, and regional rail, the project will identify similarities and differences in how residents of the two cities use public transportation. By evaluating transit usage patterns, the project seeks to better understand how transit systems perform in two major metropolitan areas with different population sizes, infrastructure systems, and commuting behaviors.

Goal with the data - 
Compare monthly ridership trends between the transit systems in NYC and Philadelphia.
Analyze how different transportation modes (bus, subway, commuter rail) are used in each city.
Suggest improvements to public transportation systems in the end? Ex - public opinions biggest issues with public transportation - what needs to be improved based on what we found in the data analyzing) Philadelphia biggest issue vs. NYC 

Literature Review: 

- Previous Research: 
Previous research on urban transportation systems suggests that several economic and social factors influence public transit ridership. Factors such as
changes in commuting preferences
economic conditions
Public opinions on safety
reveal a significant effect on how frequently people use public transportation
systems. Using sources that analyze overall public transportation usage and transit
trends, rather than focusing only on New York City and Philadelphia, helps provide a
broader explanation of urban transportation patterns and commuting behavior.

Data Understanding and Preparation 

- Dataset Specification: 

Data Set 1. NYC Transit Data: Data from the Metropolitan Transportation Authority includes monthly ridership statistics for multiple transit services including:
Subway
Bus
Long Island Rail Road
Metro-North Railroad
Access-A-Ride
Bridges and Tunnels
The dataset covers January 2021 through December 2025.

Data Set 2. SEPTA Philadelphia Transit Data: The second dataset comes from the Southeastern Pennsylvania Transportation Authority: 
Buses 
Regional Rail 
Subway + Trolley Systems 

- Initial Data Exploration:
Data Cleaning: 
Converting dates into a consistent monthly format
Standardizing column names so we can compare each line of transportation (Subway Ridership in July 2021 NYC vs. Subway Ridership in July 2021 SEPTA) 

Key Variables
Date / Month  - datetime.now() , 
Transit mode (bus, subway, rail)
Number of passengers or ridership count

Summary Statistics and Visualization
Line charts to show ridership trends over time (Increased or decreased)
Bar charts comparing transportation modes (ex - More ridership on buses than trains) 
Summary statistics (mean, median, standard deviation - .describe() ) 

Notes - Will probably have to make 4 new data frames based on mode ride ex- 
New_df_trains = Column 1 - nyc trains vs column 2 septa trains 
New_df_buses = Column 2 - nyc buses vs column 2 septa buses 

- Feature Selection/Engineering: 
For this project, we will focus on selecting the most relevant variables from the datasets that help explain public transit usage. The main variables we plan to use include date (month and year), transit mode (bus, subway, or rail), and ridership counts. These variables are directly related to the goal of the project, which is to compare how people use public transportation in New York City and Philadelphia. By focusing on these key variables, we can better track ridership patterns and compare transportation usage between the two cities.
In addition to selecting important variables, we may also create new features to improve the analysis. For example, we may calculate monthly ridership totals for each transit mode, measure percentage changes in ridership from one month to the next, or group data by year or season to identify long-term trends. These new features will help make patterns in the data easier to see and will allow us to compare transit usage more clearly. Creating these features will help us better understand how ridership changes over time and provide useful insights when comparing the public transportation systems in both cities.
4. Methodology: 
To analyze public transit ridership patterns in New York City and Philadelphia, this project will use descriptive statistics, trend analysis, regression analysis, and comparative analysis. These methods will help identify patterns in ridership and show how transportation usage differs between the two cities.
Descriptive Statistical Analysis
The first step will be to use descriptive statistics to summarize the data. This includes calculating values such as the mean, median, minimum, maximum, and standard deviation for each transportation mode, including buses, subways, and regional rail. These statistics will help us understand the general ridership patterns and see how usage differs across transit modes and cities.
Data Visualization and Trend Analysis
Data visualization will be used to better understand ridership trends over time. Visual charts make it easier to see patterns in the data.
The project will use:
- Line charts to show monthly ridership trends
- Bar charts to compare transportation modes
- Comparison graphs to show differences between NYC and Philadelphia

This will help us see whether ridership is increasing, decreasing, or staying the same over time.
- Regression analysis may be used to study how ridership changes over time. This method helps measure the relationship between time and ridership levels. For example, regression can help show whether ridership is gradually increasing or decreasing across the months in the dataset.
Comparative Analysis
- Comparative analysis will be used to directly compare transportation usage between the two cities. The data may be separated by transit mode so that similar services can be compared more easily. For example, NYC subway ridership can be compared with Philadelphia’s subway or trolley system, while bus ridership can also be compared between the two cities.
- Hypothesis Testing helps to determine whether differences in ridership between the two cities are statistically meaningful.

Statistical tests such as a t-test may also be used to evaluate these differences.
Evaluation Metrics
Several metrics will be used to evaluate the results of the analysis and to confirm that the results are supported by the data. These may include:
- R-squared to measure how well regression explains ridership trends
- Correlation values to show relationships between variables
- p-values to determine whether results are statistically significant

Why These Methods Are Suitable
- These methods are suitable because the main goal of this project is to analyze and compare ridership patterns in two major transit systems. Descriptive statistics and visualizations help summarize the data and make trends easier to understand. They also allow the group to clearly communicate the results of the analysis.
- Regression analysis helps measure how ridership changes over time and provides a more detailed way to study trends in the data. Comparative analysis is important because the main focus of the project is to examine the differences between New York City and Philadelphia’s transit systems.
- Adding hypothesis testing and evaluation metrics also strengthens the analysis. These methods help confirm whether the patterns we observe in the data are statistically meaningful. Overall, using these techniques will allow the group to explore ridership patterns, compare the two cities, and draw meaningful conclusions from the data.

Dataset Sources: 
NYC Transit Dataset
Metropolitan Transportation Authority. (2025). MTA regional transit ridership beginning
     2021 [Data set]. U.S. Data.gov. https://catalog.data.gov/dataset/mta-regional-transit-      
     ridership-beginning-2021 

Philadelphia Transit Dataset
Southeastern Pennsylvania Transportation Authority. (2025). Average daily ridership by 
      service [Data set]. SEPTA Open Data Portal. https://data-septa.opendata.arcgis.c
      om/datasets/average-daily-ridership-by 

Literature review sources: 
Source #1 - 
Previous research has identified factors that influence public transit ridership:  population density, automobile ownership, transit fares, and service frequency. Cities with higher population density and fewer car-owning households tend to experience higher levels of public transit use (Taylor & Fink, 2003).

Taylor, B. D., & Fink, C. N. Y. (2003). The factors influencing transit ridership: A review           
     and analysis of the ridership literature. University of California Transportation     
     Center. https://escholarship.org/uc/item/3xk9j8m2 
 
