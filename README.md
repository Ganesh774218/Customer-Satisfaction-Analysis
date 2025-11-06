# Customer-Satisfaction-Analysis

Customer Satisfaction Analysis:

****Overview**
Customer Satisfaction Analysis involves collecting, analyzing, and interpreting data on customer experiences and perceptions through surveys, feedback forms, ratings, and reviews.
By identifying key drivers of satisfaction and dissatisfaction, businesses can make informed decisions to improve products, services, and customer interactions.

It helps retain customers, boost loyalty and advocacy, drive sales growth, and gain a competitive edge, which ultimately enhances overall business performance and customer experience.

To get started with the task of Customer Satisfaction Analysis, we need a dataset based on customer satisfaction and feedback. I found an ideal dataset for this task, 
which contains features like:

CustomerID: Unique identifier for each customer.

Age: Age of the customer.

Gender: Gender of the customer (Male/Female).

PurchaseAmount: Total amount spent by the customer.

PurchaseFrequency: Number of purchases made by the customer.

ProductQualityRating: Customer rating for product quality (1-5).

DeliveryTimeRating: Customer rating for delivery time (1-5).

CustomerServiceRating: Customer rating for customer service (1-5).

WebsiteEaseOfUseRating: Customer rating for website ease of use (1-5).

ReturnRate: Proportion of products returned by the customer.

DiscountUsage: Amount of discount used by the customer.

LoyaltyProgramMember: Whether the customer is a loyalty program member (Yes/No).



**Libraries Used for manipulation and visualization:**
Pandas
Seaborn
Numpy 
Matplotlib



**Analysis Steps:**

Data Loading: Reads dataset with pandas.

Data Inspection: Uses .info() and .describe() to understand data structure and basic stats.

Descriptive Statistics: Calculates averages, ranges, and variability for numeric columns.



****Visualization:**
Histograms and bar charts for age, ratings, and purchase behavior.

Possibly correlation heatmaps (common with sns.heatmap()).

Interpretation: Markdown sections summarize insights such as:

Average customer age ≈ 44 years.

Average purchase amount ≈ $1065 (high variability).

Average rating ≈ 3/5 across metrics → moderate satisfaction.

Return rate ≈ 25%.

Discount usage ≈ $251 on average.



**Insights Summary:**
Customer base is diverse across ages.
Spending and satisfaction vary significantly.
Moderate satisfaction levels suggest room for service improvements
Discount and return behavior show variability, indicating different customer segments.
