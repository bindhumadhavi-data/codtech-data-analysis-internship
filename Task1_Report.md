#Task 1 – Big Data Analysis using PySpark/Dask
##1. Introduction
The goal of this task is to perform initial exploration and analysis on a large-scale dataset.
The dataset chosen is the **NYC Yellow Taxi Trips (January 2016)**. With over **10.9 million records**, it is highly suitable for **big data analysis** due to its size and real-world relevance.

##2. Tools & Technologies
•	Python (Jupyter Notebook)
•	PySpark / Dask – for scalable big data handling
•	Pandas – data manipulation
•	Matplotlib & Seaborn – data visualization

##3. Dataset Overview
•	**Rows**: 10,906,858
•	**Columns**: 19
•	**Key features**: Pickup & dropoff times, passenger count, trip distance, fare, tip, total amount, payment type
This dataset enables exploration of **travel behavior, revenue, demand patterns, and correlations** in NYC taxi services.

##4. Data Exploration & Analysis
###4.1 Row Count
•	Verified dataset has **over 10M rows** → confirms big data use case.
###4.2 Group By Analysis
•	Example: Average fare by passenger count.
•	Insight: Most rides are single-passenger; fares scale with trip distance.
###4.3 Filtering
•	Trips > 100 miles = rare outliers.
•	Majority of trips < 10 miles.
###4.4 Trends & Summaries
•	**Peak hours**: 6 PM – 9 PM
•	**Lowest demand**: 4 AM – 5 AM
•	**Payment preference**: 65.8% credit card vs 33.6% cash
(Visuals: trips by hour, trips by day, payment type bar chart, correlation heatmap)

##5. Key Insights
•	Most trips are **short, single-passenger rides.**
•	**Evenings/weekends** = peak demand.
•	**Trip distance** is the strongest revenue driver.
•	**Credit cards dominate** over cash.
•	Outliers **(like 8M miles trips)** stress the need for cleaning.

##6. Conclusion
•	Task 1 demonstrated **big data exploration** using PySpark/Dask.
•	The dataset’s **10M+ rows** required scalable tools.
•	Insights revealed important **patterns in demand, revenue, and behavior.**

##7. Next Steps
•	Proceed to **Task 2 – Machine Learning Model**
o	Data cleaning & preprocessing
o	Feature engineering
o	Model training & evaluation (e.g., predicting fare amount)

