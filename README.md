Description
This Python script processes customer transaction data to calculate key RFM metrics, which help businesses analyze customer behavior and determine their value.

Key Functionalities:
Dataset Handling:

The script loads transaction data from a CSV file named Online_Sales.csv using pandas.
Ensures the Transaction_Date column is converted into a datetime format to perform date-based calculations.
RFM Metric Calculation:

Recency: Calculates the number of days since the customer's most recent purchase. The reference date is set as the latest date in the dataset.
Frequency: Counts the number of unique transactions per customer (Transaction_ID).
Monetary Value: Computes the total spending (Avg_Price) of each customer over the observed period.
Revenue: Represents the total monetary value, equivalent to the Monetary metric.
Customer Segmentation:

Groups data by CustomerID to compute the above metrics for each individual customer.
Outputs the processed data in a structured format for further analysis or visualization.
Sorting and Ranking:

Customers are sorted based on their computed values (e.g., highest monetary value or frequency) to identify top-performing or high-value customers.
Libraries Used:
pandas: For data manipulation and computation of metrics.
Applications:
Customer Segmentation: Identify high-value customers or those at risk of churning.
Marketing Campaigns: Design targeted strategies for different customer segments.
Business Decision-Making: Understand customer behavior and prioritize resources accordingly.
