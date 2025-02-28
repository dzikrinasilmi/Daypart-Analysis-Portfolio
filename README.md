# Daypart-Analysis-Portfolio

## Introduction
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

Dataset Information
-	Date: the date the customer made the transaction
-	Time: the time at which the customer made the transaction
-	Daypart: the time segments in which the customer made the transaction (Morning, Noon, Afternoon, evening)
-	Category: the category of the item the customer ordered during the transaction (Snack, Coffee, Drink, Food)
-	Item: the name of the food or drink the customer ordered during the transaction
-	Quantity: the number of items the customer ordered
-	Total Price: the total price of the item purchase
-	Transaction Type: the type of transaction selected by the customer (Dine-in, Take-away, Delivery)

## Result
### 1. What is the pattern of customer visits and transactions in each time segment (morning, noon, afternoon, night)?
-	Based on the result of total sales and total transactions per daypart, Morning and Evening are the highest peak sales and transactions. Noon daypart experienced a significant drop in total sales and transactions, which could be due to this daypart, customers moving to other places or there is a change in customer trends. While the afternoon tends to be stable, which means it has the potential to increase both sales and transactions.
![Total Transaction per Daypart](https://github.com/user-attachments/assets/ff2d0520-cf45-41db-84de-a17fbb5b5626)
![Total Sales per Daypart](https://github.com/user-attachments/assets/5a31705e-782a-49ab-ace0-e82fb1ba8aa1)
-	Based on the average purchase per transaction graph, it shows that the Noon daypart has the highest average transaction even though the number of purchases is less, indicating high purchasing power. Evening attracts many customers but they tend to buy only one item, indicating an opportunity for upselling. Morning has a high transaction volume with a smaller average purchase than Noon. And Afternoon has the lowest average purchase, so there is still potential for improvement.
![Average Sale per Transaction per Daypart](https://github.com/user-attachments/assets/f19b2112-8dde-4752-b7ab-b212480db184)

### 2. What is the most ordered menu in each time slot?
-	The most ordered menu in the morning is Latte with a total order of 89 items, in the Noon is Salad with 39 items, Afternoon is Americano with 52 items, and in the evening is dominated by Cappuccino with 55 items of total orders.
![most ordered menu](https://github.com/user-attachments/assets/9600ce35-50c2-469e-8b02-b55a3f8ae324)
-	From the information above, it is known that coffee is the main product ordered by customers in almost every daypart segments.
-	By looking at the dominance of salad orders during the Noon segment, it shows that daytime customers are more focused on food, especially a heavy food compared to coffee. This is what causes the average sales per transaction to be higher in the Noon segment even though there is a significant decline overall.

### 3. Are there any differences in transaction patterns between weekdays and weekends in each time slot?
-	Based on total transaction per daypart, transactions that take place on weekdays are much higher than weekends in each daypart segment, the difference can reach twice as high. This shows that the average customer comes more during weekdays. ![Total Transactions per Daypart (Side by Side with Labels)](https://github.com/user-attachments/assets/3ed325c6-2159-41aa-b0e8-90ecd0cbdee7)

-	Total sales per daypart also show a similar graph, where total purchases are more during weekdays than weekends with a difference that reaches twice. This can be caused by the large number of office worker customers who come and make purchases during weekday. ![Total Sales per Daypart (Side by Side with Labels)](https://github.com/user-attachments/assets/c48a6b70-5918-4be3-a15d-2e2b921aad12)

-	The average sales per transaction shows similar results between weekday and weekend in each daypart segment, but the average on weekends is higher. This means that the customers tend to buy more items on weekends, which can be inferred that they also tend to spend more time at Café on weekends, for example hanging out with friends at the Café. ![Avg Sale per Transaction per Daypart (Side by Side with Labels)](https://github.com/user-attachments/assets/b72d3ee6-79d9-4134-9fa5-c6f07f599b58)

### 4. How does the number of dine-in, take-away, and delivery transactions compare in each daypart?
![Comparison transaction type](https://github.com/user-attachments/assets/80d7bd98-c875-4a13-b7f9-98c427997038)

-	From the visualization, it is known that customers prefer to choose Dine-in compared to other transaction types, especially during the Morning and Evening. This can be seen from the significant difference in graphs between Dine-in, Take-away, and Delivery.
-	The Take-away transactions type also quite widely chosen especially in the Morning, it is likely that these customers are office workers who stop by to buy coffee and will enjoy it on the way or when they get to the office.
-	While Delivery is a transaction type that is not yet in high demand by customers, as seen from the relatively low total transaction types in each daypart segments.

## Insight
-	The drop in turnover most likely comes from significantly reduced in Noon segment revenue. This can have an impact on long-term profitability.
-	The Café’s revenue is still dependent on office worker customers during the morning rush, which means there is a high risk if the WFH (Work From Home) trend picks up again.
-	Total transactions and sales on weekends still have lower traffic than weekdays. This shows that the Café has not been able to attract a wider market on holidays.
-	The Afternoon segment shows potential to attract new customers, but there is no effective strategy to maximize revenue from this daypart segment.
-	The Café does not yet have an optimized marketing strategy for the Delivery transaction type.

## Recommendation
-	Improve sales strategies in the Noon segment, such as holding lunch promos to attract customers or collaborating with neighboring companies by offering catering packages or special promo vouchers for employees who work at the office.
-	Optimize the potential for increased sales in the Afternoon, such as holding B1G1 (Buy 1 Get 1) promo during the segment periods or working together as a venue organizer for community events that take place in the Afternoon.
-	Increase repeat orders and transactions in the Evening segment, for example by creating a bundle of popular evening menus. This can increase transaction and sales opportunities without the need to increase customer traffic.
-	Increase sales via Delivery service with various activities, such as optimizing account management in the delivery application to attract an online buyers, providing shipping discount for minimum purchases, and actively conducting online promotions to add a wider range of customers.
