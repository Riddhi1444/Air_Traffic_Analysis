# Air_Traffic_Analysis

## Introduction:
This report provides a comprehensive analysis of air traffic to uncover trends, passenger flow patterns, and regional activity distribution for informed decision-making in the aviation sector. Understanding air traffic flow and its associated factors is crucial for improving operational efficiency, passenger experience, and resource allocation. This project seeks to address these challenges by analysing the provided air traffic data.

## Objective:
The objective of the report is to:
•	To identify the busiest airlines and regions. 
•	To analyse passenger trends across time (monthly and yearly).
•	To explore terminal and boarding area usage.
•	To detect seasonal or geographical trends affecting passenger traffic.

## Data Overview:
•	The dataset consists of information about passenger traffic based on different Airlines, across different months of the years.
•	It includes features such as Activity Period, Operating Airline, Operating Airline IATA Code, Published Airline, Published Airline IATA Code, GEO Summary, GEO Region, Activity Type Code, Price Category Code, Terminal, Boarding Area, Passenger Count, Adjusted Activity Type Code, Adjusted Passenger Count, Year, Month.

## Data Preparation:
•	Libraries like Pandas, NumPy, Matplotlib.pyplot, seaborn were imported and the data was loaded from a csv file using the “read_csv” function.
•	Data was checked for null values using the “isnull()” function and null values were filled by “fillna()” .
•	All Columns were checked for unique values with the help of “unique()”  and the inappropriate values were replaced by appropriate values using “replace()”.

## Exploratory Data Analysis (EDA):
•	The dataframe information was explored using “df.info()” and datatypes of the columns were checked using “df.dtypes” and were changed when needed.
•	Column names were retrieved using “df.columns”.
•	“head()” function was to display first few rows of the dataset to get the glimpse of the data.
•	The statistics were checked for all numeric columns using “describe()” to get more insights about the features like their range(min, max)values, mean, standard deviation etc., this helped in knowing the skewness of the data and presence of outliers.

## Temporal Analysis:
•	Region wise and activity type wise contribution to passenger count was found using “n.largest(), n.smallest() and countplot()” .
•	Evolution of passenger traffic over years and month was found using “pivot table” and then correlation was found using “heatmap”.
•	The peak and drop in passenger count with respect to specific month or season was found using “lineplot”.

## Airline Analysis:
In this passenger traffic distribution among different airlines was observed using “barplot”  and the airline with the highest and lowest passenger traffic were found out using “n.largest(), n.smallest()” .
Terminal and Boarding Area Analysis:
The busiest Terminals and Boarding Area and the difference in there usage was found by “barplot”.

## Conclusion:
The air traffic dataset analysis revealed key patterns and trends across airlines, regions, and time periods:
•	Top-performing airlines and regions were identified based on passenger volume, enabling targeted resource allocation and strategic partnerships.
•	Monthly and yearly passenger trends showed significant seasonal fluctuations, with clear peak periods that can inform staffing, scheduling, and capacity planning.
•	Terminal and boarding area usage analysis highlighted specific high-traffic zones, pointing to potential areas for operational efficiency improvements.
•	Correlation and time-series analysis demonstrated consistent growth in passenger numbers post-specific periods, which may align with external factors such as policy changes or global events.
These findings can support data-driven decision-making across airline operations, infrastructure planning, and customer service strategies.
