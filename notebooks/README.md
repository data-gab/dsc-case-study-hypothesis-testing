# Case Study Hypothesis Testing
***

## Introduction
For this case study, the supplier company Northwind has given us access to their database in order to determine interesting relationships. Hypothesis tests were conducted and normality tests along with visualizations were used to answer questions.
***

## Information About Database 
![northwindERD.png](attachment:northwindERD.png)

The image above is the Northwind database schema.
The database contains the following tables:

    - Products
    - Suppliers
    - Region
    - Orders
    - Order Details
    - Categories
    - Employees
    - Employee Territories
    - Territories
    - Customers
    - Customer Demographics
    - Shippers

These tables were used to answer the following questions in order to determine interesting relationships.
    

***
## Question 1: Is there a difference in quantity of products sold by discount rate? 
**Paired T-Test**

**H0**: There is no difference in the quantity of products sold based on how much they are discounted

**HA**: More products are sold when they are discounted versus when they are full price

![q1%20dist%20discounts%20quantity.png](attachment:q1%20dist%20discounts%20quantity.png)

***Figure1: Quantity vs. Probability***

![q1%20sample%20dist%20seaborn.png](attachment:q1%20sample%20dist%20seaborn.png)

***Figure 2: Quantity vs. Probability***

![q1%20sample%20dist%20plotly.png](attachment:q1%20sample%20dist%20plotly.png)
***Figure 3: Quantity vs. Probability***

### Conclusion
We have 95% confidence that products sold with a discount will have a higher mean quantities sold than products sold without a discount.

***
## Question 2: Is there a difference in number of orders and territory?

### Turkey Test
H0: There is no difference between average order prices in each territory.

HA: Different territories generate significantly different sales revenue per order.

![q2%20dist%20territories.png](attachment:q2%20dist%20territories.png)
***Figure 4: Order Price vs. Proabability***

### Conclusion
We fail to reject the null hypothesis and conclude that there is no significant difference between average order prices in each territory.

***
## Question 3: Is there a difference in Sales per Order between Summer and other seasons?
**H0**: There is no difference between Sales per Order during the Summer and Sales per Order NOT during the summer

**HA**: The Sales per Order during the Summer is different from Sales per Order NOT during the summer

![Question3_Distributions_whitebackground.png](attachment:Question3_Distributions_whitebackground.png)
***Figure 5***

![Question3_Sample_Mu_Distributions.png](attachment:Question3_Sample_Mu_Distributions.png)

***Figure 6***

### Conclusion
We can state with 95% confidence that orders created durign the Northern Hemisphere Summer have Lower mean "Sale" than orders created during times of the time of year.
