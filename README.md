# Franchise_Stakeholder_EDA

**Exploratory Data Analysis**
**Franchise EDA**
**Steps for Analysis:**
1. Data Upload
2. Data Cleaning/Quality Check
3. Data Wrangling
4. Univariate/Bivariate/Multivariate Exploration
5. Address Stakeholder Questions and Key Takeaways

**Questions Posed by Initial Query:**

**1) What is the most popular item at Burgers & Shakeland?**

Shakes

**2) Which location is the busiest? Does the answer to this question change throughout the day?
**
State Street is the business location. The following visualizations will demonstrate that State Stret's sales are higher. It should be noted that the winner for busiest hour does trade off three times per day at/around hours 11am, 4pm, and 9pm.

The order of visualizations which follow are:
A) Historical Daily Sales Trend

B) Historical Hourly Sales Trend

C) Union Heights Hourly Sales Trend

D) State Street Hourly Sales Trend

E) State Street vs Union Heights Hourly Sales

F) State Street vs Union Heights Hourly Moving Average

**3) A combo meal consists of 1 Burger, 1 Fry, and either a drink or a shake. How many Combo meals were sold from the State Street location in April?**

This is a tricky question, as there is not enough data to support the answer of this question within the transaction data. In fact, to assume a relationship between transaction time and item number sold is to commit a fallacy: correlation does not prove causation. Another fallacy which would occur in answering this question would lie in the relationship of item name and item_ID. This would lead to the fallacy of the cart before the horse. This would occur because a relationship would be assumed by variables time, item, and possibly employee name. Just because item_id has in common an instance (time) with another feature (row) does not necessarily mean that the items were rung up together and are therefore a combo. Thust the question is not answerable.

The only way to answer this question with integrity is to re-mine the data source for a more logical variable order number or combo number. Features (rows) could then be grouped by order number and assessed according to stakeholder interest in order to asnwer this question.

**Attempt at question:**

According to the above program, there was a maximum of 657 possible combos (unproven due to fallacy). The only way to say with certainty if items purchased were a combo or not would be the variable order number.
