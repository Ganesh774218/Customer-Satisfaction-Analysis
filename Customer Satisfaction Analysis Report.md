### Customer Satisfaction Analysis



**🧩 1. Objective**



The notebook aims to analyze customer satisfaction data to identify behavioral patterns, spending trends, and service quality perceptions among customers.

It explores demographic, transactional, and satisfaction-related features to uncover actionable insights for improving customer experience and business performance.4









**2. Dataset Overview**





Key Variables



Category	                              Columns	            Description



Demographics	                                   Age	            Age of the customer (18–69 years)



Transaction Behavior      	         PurchaseAmount	            Total amount spent (in USD)

&nbsp;	                                 PurchaseFrequency	    Number of purchases per customer

&nbsp;                                        



Satisfaction Ratings (1–5 scale)	ProductQualityRating,       Ratings representing customer satisfaction across service areas

&nbsp;                                       DeliveryTimeRating,

&nbsp;                                       CustomerServiceRating,

&nbsp;                                       WebsiteEaseOfUseRating	



Post-Purchase Behavior	                ReturnRate	            Fraction of items returned (0–0.5)

&nbsp;	                                DiscountUsage	            Average discount used by the customer (in USD)









**Descriptive Statistics Summary**



Feature	                                     Mean / Observation	                      Notable Points

Age                                              44 years                             Range 18–69; balanced age distribution

Purchase Amount                                  ~$1065                               High standard deviation → large variability in spending

Purchase Frequency                            ~14 purchases                           Some customers up to 29 purchases

Ratings (avg)                                 Around 3/5                              Indicates moderate satisfaction

Return Rate                                    ~25%                                   Up to 50% for some customers

Discount Usage                                 ~$251                                  High variability — some rely heavily on discounts













**4. Exploratory Data Visualization**



Visualization Code Used

numerical\_columns = \[

&nbsp;   'Age', 'PurchaseAmount', 'PurchaseFrequency',

&nbsp;   'ProductQualityRating', 'DeliveryTimeRating',

&nbsp;   'CustomerServiceRating', 'WebsiteEaseOfUseRating',

&nbsp;   'ReturnRate', 'DiscountUsage'

]



plt.figure(figsize=(15, 20))

for i, col in enumerate(numerical\_columns, 1):

&nbsp;   plt.subplot(5, 2, i)

&nbsp;   plt.hist(data\[col], bins=20, edgecolor='k', alpha=0.7)

&nbsp;   plt.title(f'Distribution of {col}')

&nbsp;   plt.xlabel(col)

&nbsp;   plt.ylabel('Frequency')

plt.tight\_layout()

plt.show()







**Insights from Histograms:**



Age: Even distribution with small peaks in the 30s and 60s.



Purchase Amount: Right-skewed — majority spend under $1000.



Purchase Frequency: Peaks near 10 and 20, suggesting distinct shopper groups.



Ratings: Distributions center around 3 (neutral/moderate satisfaction).



Return Rate: Peaks near 0.1 and 0.4 — some customers highly likely to return products.



Discount Usage: Uniformly spread — no dominant pattern.



**🧩 Interpretation:**

Customers show diverse behaviors — while spending and engagement vary widely, satisfaction is generally moderate, hinting at improvement opportunities in product quality, delivery, and service.









**Analytical Findings**

Customer Profile Insights



Middle-aged customers (35–50) form a core demographic.



Spending patterns vary widely, suggesting segmentation potential (e.g., budget vs. premium buyers).



Frequent buyers (high purchase frequency) might be linked to higher satisfaction — to be validated via correlation analysis.



Satisfaction Dynamics



Ratings around 3 suggest neutral or average satisfaction across service dimensions.



Improvement in delivery time and customer service could raise overall experience.



Return \& Discount Behavior



High return rates may indicate product quality or expectation mismatch.



Strong discount usage variability suggests different price sensitivities.









**Key Insights Summary**

Theme	                            Insight	                         Implication

Customer Age        Balanced age groups with peaks in 30s \& 60s          Marketing strategies should cater to both young professionals and older customers

Spending Patterns   Most spend < $1000                                   Potential for upselling via loyalty or premium offers

Purchase Behavior   Two clusters (light \& frequent buyers)               Segment customers based on engagement

Satisfaction Levels                Avg ≈ 3/5                             Customer satisfaction can be improved

Return Behavior                     Avg 25%                               Indicates product or expectation issues

Discount Usage              High variability                              Identify price-sensitive vs. value-driven customers







**Conclusion:**

The Customer Satisfaction Analysis project effectively explores behavioral and satisfaction patterns within a retail or e-commerce dataset.

It identifies moderate satisfaction levels, spending diversity, and return-rate challenges — offering a foundation for customer segmentation, retention strategy, and service improvement initiatives.

