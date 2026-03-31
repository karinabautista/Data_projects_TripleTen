# Customer Segmentation Analysis for Zomato 

This project explores Zomato’s customer base to better understand who their customers are,
how they behave, and how they can be grouped into meaningful segments. By analyzing
customer demographics and purchasing patterns, the goal is to identify key differences in
customer activity, highlight high-value users, and uncover opportunities to improve customer
retention and engagement.

---

## Data Preparation & Methodology

To prepare the dataset for analysis in Tableau, the Users table was combined with the Orders
table using a LEFT JOIN. This approach ensured that all customers were retained in the
analysis, including users who have not yet placed an order. These customers were later
categorized as part of a “No Orders” segment, which helped provide a complete view of
Zomato’s customer base.

After joining the tables, the dataset was reviewed for inconsistencies such as missing values
and incorrect data types. Date fields were validated to ensure they were properly formatted for
time-based analysis, and customer demographic fields (such as age and gender) were checked
for usability in segmentation.

Because the LEFT JOIN produced null order fields for customers with no purchase history,
records with null order dates were excluded only when building the Orders Over Time
visualization to ensure the trend line reflected actual purchasing activity. A year-level date filter
was also added to allow stakeholders to explore purchasing trends across different time periods
more easily.

To support customer segmentation, several calculated fields were created in Tableau. These
fields were used to measure purchasing behavior and categorize customers based on their
activity. Customers were segmented into behavioral groups, including:

- No Orders (users with no purchase history)
- One-Time Customers (customers with exactly one order)
- Repeat Customers (customers with multiple orders)

Additionally, an “Orders per Customer” metric was created to measure purchase frequency at
the individual customer level. This field was used to evaluate repeat behavior and identify
high-value customers based on order volume.

Segmentation in this project was primarily based on:

- Demographics (age and gender)
- Purchase frequency / repeat behavior
- Customer activity over time

These preparation steps and calculated fields allowed the dashboard to accurately reflect
customer behavior and support meaningful segmentation analysis.

---

## Dashboard Walkthrough / Findings

### Customer Overview (KPI Summary)

The dataset contains 100,000 customers. The average customer age is 25, and customers
place an average of approximately 1.5 orders per customer, indicating that while many users
order only once, there is a significant portion returning for at least a second purchase.

Additionally, 44.5% of customers are repeat purchasers, suggesting that nearly half of the
customer base returns to place at least an additional order.

These metrics provide an initial view of customer demographics and purchasing behavior. They
support segmentation based on age and purchase frequency, which can help identify high-value
customers and inform targeted engagement strategies.

---

### Customer Demographics: Gender

The customer base is comprised of 42.8% Female and 57.2% Male. Given a fairly balanced
distribution across genders, these insights suggest that engagement strategies should target
both groups to maximize reach and retention. Gender can also be used as a segmentation
dimension to tailor campaigns, promotions, or personalized offers to each group.

---

### Customer Demographics: Age Distribution

The majority of customers fall within the 22–25 age range, with 23 being the most common age.

While the overall average customer age is 25 (from the KPI overview), this shows that a large
portion of the customer base is slightly younger than the average. Engagement efforts and
campaigns targeting this 22–25 age group may maximize retention and repeat purchases.

Beyond age 25, customer counts gradually decline, with a smaller increase around age 32
before dropping sharply at 33. This suggests that tailored campaigns for older age groups could
help expand engagement beyond the primary younger segment.

---

### Purchasing Trends Over Time

The line chart of orders over time shows a gradual increase in total orders until June 2018,
followed by a gradual decline with occasional spikes through May 2020.

While there is evidence that many customers place repeat orders, the overall trend indicates
less engagement over time. This suggests that while a core base of repeat customers exists,
additional strategies may be needed to encourage continued ordering and retention,
particularly for customers who have lapsed.

---

### Customer Segmentation: Purchase Frequency

The purchasing frequency chart shows that Repeat Customers are the largest group, followed
by One-Time Purchasers, and then No Purchases. There is roughly a 10,000-customer gap
between each category.

This indicates that a good majority of purchasing customers return at least once, highlighting
the potential for targeted campaigns to further encourage repeat orders.

Segmenting customers by purchasing frequency allows Zomato to:

- Identify high-value, repeat customers for loyalty programs or personalized offers
- Re-engage one-time customers with promotions or incentives
- Understand potential churn among customers who haven’t yet made a purchase

---

## Customer Segmentation Summary

Based on the analysis, customers can be grouped into distinct segments using demographics
and purchasing behavior:

### No Order Customers
Users who have not placed any orders represent an opportunity for conversion. These
customers may require incentives or onboarding strategies to encourage their first purchase.

### One-Time Customers
Customers who have only placed one order show initial engagement but may not yet be fully
retained. This group represents an opportunity to increase repeat behavior through targeted
promotions or follow-up engagement.

### Repeat Customers
This is the largest segment, indicating a strong base of returning users. These customers are
the most valuable, as they contribute consistently to overall order volume.

Additionally, demographic insights show that the customer base is primarily composed of
younger users (ages 22–25), with a relatively balanced gender distribution. These
characteristics can be used to further refine segmentation and target specific customer groups
more effectively.

---

## Conclusions & Recommendations

This analysis reveals that while Zomato has a solid base of repeat customers, overall
engagement shows signs of decline over time. This suggests that maintaining and increasing
customer retention should be a key focus.

Based on these findings, the following recommendations are proposed:

- Strengthen Retention Strategies  
  Since repeat customers make up a significant portion of the customer base,
  implementing loyalty programs, personalized offers, or rewards systems could help
  maintain and increase engagement.

- Re-engage One-Time Customers  
  Target customers who have only ordered once with follow-up promotions, discounts, or
  reminders to encourage additional purchases.

- Convert Non-Purchasing Users  
  Customers who have not yet placed an order represent a key growth opportunity.
  Introductory offers or first-order incentives may help convert these users into active customers.

- Target Key Demographics  
  With the majority of customers falling within the 22–25 age range, marketing campaigns
  can be tailored to this demographic to maximize engagement and effectiveness.

- Address Declining Order Trends  
  The decrease in orders over time suggests a need to investigate potential causes, such
  as changing customer preferences or increased competition, and to implement
  strategies to sustain long-term growth.
