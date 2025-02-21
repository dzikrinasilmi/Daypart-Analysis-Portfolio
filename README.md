# Daypart-Analysis-Portfolio

## introduction
Daypart analysis is a data analysis method used to segment and evaluate business performance based on time of day. This analysis aims to understand patterns of customer behavior across different time periods.
### Key components in Daypart Analysis
-	Daypart: time of day divided into segments
-	Collect data: retrieve transaction data based on timestamp
-	Identifying time patterns: grouping data in a specific daypart segment
-	Analyzing trends: analyzing time case when there is a spike or drop in activity
-	Adjusting strategies: implementing operational and marketing strategies based on result from analysis
-	Monitor and evaluate: test the effectiveness of the strategy and make adjustment where necessary

## Study Case
### Objective
coffeehouse Café, a popular coffee shop in the city center, has seen its daily turnover drop by about 20% in the past three months, especially on weekdays. The number of customers has remained relatively stable, but sales have been declining. The owner has tried various promotional strategies but the results were not as expected, so it was necessary to find the main cause of its problem.
As a first step, the owner divides the time of day into segments and collects transaction data for the past 2 months according to the time segments. The results are:
-	Morning (07:00 – 10:00): stable sales (30% of the daily total)
-	Noon (10:00 – 14:00): significant decrease (only 15% of the daily total)
-	Afternoon (14:00 – 17:00): stable but not increasing
-	Evening (17:00 – 21:00): crowded but the average purchase per customer decreased
### Business Problem
-	Lost revenue from daytime customers that led to a significant decline
-	Untapped business opportunities in the afternoon
-	Relatively low conversion per customer in the evening
### Key Questions
-	What is the pattern of customer visits and transactions in each time segment (morning, noon, afternoon, night)?
-	What is the most ordered menu in each time slot?
-	Are there any differences in transaction patterns between weekdays and weekends in each time slot?
-	How does the number of dine-in, take-away, and delivery transactions compare in each daypart?
  
## Dataset
<a href="https://github.com/dzikrinasilmi/Daypart-Analysis-Portfolio/blob/main/CoffeeHouseCafeDataset.csv">Dataset</a>

Dataset explanation
-	Date: the date the customer made the transaction
-	Time: the time at which the customer made the transaction
-	Daypart: the time segments in which the customer made the transaction (Morning, Noon, Afternoon, evening)
-	Category: the category of the item the customer ordered during the transaction (Snack, Coffee, Drink, Food)
-	Item: the name of the food or drink the customer ordered during the transaction
-	Quantity: the number of items the customer ordered
-	Total Price: the total price of the item purchase
-	Transaction Type: the type of transaction selected by the customer (Dine-in, Take-away, Delivery)
