# iGnosis-Task

Step 1: Understanding the Problem Statement
Our goal is to help the marketing team identify:

  1.The top 3 most profitable products (based on total sales).
  2. The characteristics of the most loyal customers (who make the most transactions).
  3. A hypothesis on why these customers prefer certain products.

Step 2: Loading the Data
We have two datasets:

  1. purchase_behaviour.csv: Contains customer details (life stage and premium category).
  2. transaction_data.csv: Contains transaction details (product name, sales, quantity, and customer ID).

Step 3: Merging the Data
  We need to merge both datasets on the common column LYLTY_CARD_NBR (customer ID) to combine transaction data with customer   demographics.

Step 4: Identifying the Top 3 Most Profitable Products
  To determine the most profitable products, we:

  Group the data by product name (PROD_NAME).
  Sum up the total sales (TOT_SALES) for each product.
  Sort the products in descending order of total sales.
  Select the top 3 products.

Step 5: Identifying the Most Loyal Customers
We define loyal customers as those who made the most transactions.

  Count transactions per customer (LYLTY_CARD_NBR).
  Select the top 10 customers with the highest number of transactions.
  Filter the dataset to include only these customers.

Step 6: Analyzing the Characteristics of Loyal Customers
To determine their characteristics, we:

  1.Group the loyal_data by LIFESTAGE and PREMIUM_CUSTOMER.
  2.Count the number of transactions for each segment.

Step 7: Visualizing the Insights
  1. Top 3 Most Profitable Products
  We use a barplot to visualize the top 3 profitable products.

  2. Loyal Customer Segments
  We create a barplot to show the distribution of loyal customers across different life stages and premium categories.

Step 8: Formulating a Hypothesis
Based on the analysis, we hypothesize:

  Loyal customers likely belong to the "Premium" or "Mainstream" segment.
  They prefer products from strong brands or with perceived higher quality.
  Their financial capability allows them to make repeat purchases.

