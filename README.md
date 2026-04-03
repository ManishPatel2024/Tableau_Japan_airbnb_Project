# Tableau dashboard for Airbnb bookings in Japan.
In anticipation for our upcoming trip to Japan in May 2026, I wanted to create a dashboard that allows me to reasearch a good neighbourhood in Tokyo to book an Airbnb.

###💡 Key Insights & Findings
* **Total Revenue** equates to ¥17,384,262,487 for the date period September 2025 - September 2026 (includes future bookings that have not been completed yet at the time of completing this project)
* 860,452 listings across 1,150 hosts in Tokyo.
* **Kokubunji Shi** neighbourhood has the highest percentage of Airbnb availability (currently not booked) and Musashino Shi has the lowest percentage of avilability. This is across all room types.


![japan_airbnb_Tableau_project screenshot](images/japan_airbnb_Tableau_projectt.png)


### 📁 Dataset Overview
This dataset has been downloaded from https://insideairbnb.com/get-the-data/ and i chose the dataset for Tokyo, Kantō, Japan. I down loaded the following data:
*listings.csv	- Summary information and metrics for listings in Tokyo (good for visualisations)
*calendar.csv - Detailed Calendar Data

🛠️ Key Technical Skills includes:  
<ins>EDA:</ins> Aggregating data such as availability rates and converting them to a percentage to understand which neighbourhoods have higher bookings than others. Working out average price acros neighbourhoods to understand which areas are pricier to book. 

<ins>Dashboard creation</ins> Laying out key charts and tables to visualise a suitable neighbourhood to book an airbnb within. Pulling out key metrics that may be helpful. Ability to filter across chart types. For instance, if you wanted to only see Private Room Types across all metrics, you can simply click the appropriate portion of the pie chart and the other tables will update. 


### 🧹 Phase 1: Understanding the data
In this phase, I first opened the files in Microsoft Excel to review the different column types and information it held. This helped me to understand how I could potentially handle the relationships of the tables when it comes to the Tableau stage. 



### 📊 Phase 2: Exploratory Data Analysis
The first thing i wanted to explore is how i could find out the availability rate for each neighbourhood per month as a percentage. I could then use a diverging colour palette using green to indicate high avilability and red for low availbility. I created calculated columns using the IS AVAILABLE column to record binary values. 1 for yes, 0 for no. I then created another calculated column to work out an average. The resulting table in the dashboard shows airbnbs in neighbourhoods sorted from most available to least avilable across the months. I can then research further into the areas that may have high bookings to give me ideas on popular tourist attractions OR the least amount of booking areas to ensure there is availability. 

The next step was to work out average price per neighbourhood and put this into a table using the same diverging colour palette. I used the price column to calculate an average across year and months across the different neighbourhoods. In the dashboard I have sorted this from lowest average booking price to the highest. In a similar vain to the Availability Rate, I can see the neighbourhoods that are high priced or low priced. High priced area may indicate popular tourist attractions or popular city centres. 

In addition to the above, I wanted to visualise the neighbourhoods on a map so i utilised the map visualisation. 

The last 2 visualisations were the price distribution visualisation and the piechart to show the different types of rooms available in this data set. The price distribution bos plot shows which neighbourhoods lie in the average price brackets but also shows me the outliers. I can choose the various data points along the bosplot which will show me which neighbourhoods are withing the central tendency of the chart.
