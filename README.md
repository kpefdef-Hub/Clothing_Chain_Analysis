# Clothing_Chain_Analysis
Performed an analysis on the Business data, company data and US census data to advise a company experiencing stagnant sales. Using the analysis, I advised them on the best product to target at each customer


Problem Statement
An online marketing clothing chain in the United States of America was struggling to increase its sales. Overall, their sales had flatlined as such, they sought a way to boost sales across their different locations by attracting lost customers. The company would like to create a targeted marketing campaign for specific product(s) however, the management is unsure on which product (Shirt - US$25, Sweater - US$100, Leather Bag - US$1000) to focus on. My analysis aims to determine the best product to advertise to each customer.

Data
For the Analysis, three tables were leveraged including US Census Data, which contains data on average income, population, location and industry; Business Data, which includes details on the product inventory, product prices, customer rating, and the rate of product return; and Customer Data, which contained overall details about the company’s customers.

Analysis Questions
●	What is the correlation (R2 value) between sales and income?
●	What is the correlation (R2 value) between customer ratings and product return rate?
●	What are the linear regression formulas to predict customer income from customer sales?
●	Which customer do you predict has the highest income?
●	Which product will be advertised the most?

Data Cleaning
For my analysis, I imported eight tables; Average Income by State, Incomes by State, Industries, Customer List, Product Inventory, Purchase List, State List, and US Age Data. I created the Regression Table from the Customer List Table and aggregated the Average Sale (Purchases on the the Customer List Table) by State.

The Average Income by State, Income by State, Industries, Customer List, and State List tables required little data cleaning; basically reformatting of the data type. However, the Product Inventory Table and The Purchase List Table had a number of data cleaning steps to be done to make the data ready for use.
 
Product Inventory Table and Applied Steps

 
Purchase List Table and Applied Steps


Analysis

This section presents an overall explanation and view of the current state of the business.
 
General Overview Page
I used multiple cards to show the total amount of sales made, the total value of goods that we have in stock, the total ratings for our products, the total number of goods we have in stock and the rate of return of goods.
 
The DAX code to calculate the Total Value of Goods in Stock
Overall, I noticed that there was a relatively low rate of return of goods which indicates that even with the ‘good’ (not excellent) rating, customers are satisfied. In addition, in the last six months, the organisation has sold over US$250,000 worth of goods and over US$620,000 worth of goods. With the availability of the necessary data, we need to investigate if the company is having difficulty selling products or if a restock happened recently. We also need to assess the cost of holding this large amount of goods.
Moving on, the Shape Map shows an analysis of the sales by state and the table complements the shape map by showing the breakdown of each customer and the amount of money they brought into the business through purchases. The bar chart indicates a breakdown of the number of products available per stock item. The Decomposition charts show the ratings for each product. I grouped the ratings into three distinct groups (in a new column)
 
The DAX code for the New Column
Finally, I created a Gauge Chart that indicates that the company has less than its intended stock value per time. The company plans to have a stock value of at least US$700,000 per time.


 
The Second Page analyzes the relationships between variables. First, I analyzed the relationship between Average Sales and Average Income. Based on my analysis, I discovered that there is a strong positive relationship between the two variables and this is better highlighted by the R-Squared value of 0.78. As the income at a location increases, there is also a subsequent increase in the average sales. Subsequently, I also analyzed the correlation between the customer rating and the return rate. I noticed a strong inverse relationship between the two variables, as the rating increased, the return rate. This is further highlighted by the good R-Squared value of 0.69 between the two variables. These findings of the analyses reiterate my initial thought process. When the rating of a product is very good, and the customers are enjoying the product, there will be a very reduced rate of return. At the same time, when the income of a person is high, they have more funds to spend on products.
I also analyzed the top 10 states with the highest earning people. Since we know that people with a high income are more likely to spend in our shop, we need to target states with the highest earning people. These states are California, Florida, Texas, New York, Illinois, New Jersey, Pennsylvania, the District of Columbia, Maryland and Massachusetts. The last chart illustrates the average rating of each product (bars) and charts the price for each product as well (line). I noticed that Chronograph Watch and Leather Sneakers are the highest rates products and they have an average (to low) price point hence, these should be the two products the marketing team should focus on.



 
The third page analyzes the income and sales of the customer. The Map shows the average income for each state and the histogram shows the distribution of the income. I used a DAX code to classify the income into four brackets.
 
We notice from the chart that the histogram is right-skewed and there is a heavy concentration in the US$60,000 and the US$100,000 bracket.
The combination chart at the top of the Page analyzes the sales per population for each state. This shows that amount we get from each state, proportionate to their population. I saw that although the District of Columbia, Wyoming, Alaska, Vermont, North Dakota, Delaware, New Hampshire, Rhode Island, and Hawaii have low populations compared to other states, the organization gets a lot of sales from them. The chart also displays the population in a line chart.


The final page contains the analysis of the relationship between Sales and Age. While the correlation coefficient of the two variables is low, I noticed a unique relationship between them. There is a positive correlation between Sales and Age but once the age gets to between 45 - 55, the sales reduce. I extracted data from KFF Health Facts of the population by age for each state and I visualized it in the bar chart to the right. I showed the total population for each state from age 19 to 54. This is the population we expect to buy more of our products.

 
KFF State Health Facts: Link 

Answers to the Analysis Questions
●	What is the correlation (R2 value) between sales and income?
There is a positive correlation between sales and income with an R-Squared Value of 0.79.
●	What is the correlation (R2 value) between customer ratings and product return rate?
There is a Strong Negative Correlation between customer rating and return rate with an R-Squared Value of 0.69.
●	What are the linear regression formulas to predict customer income from customer sales?
The Linear Regression formula is y = mx + b
y is the dependent variable which in this case is Sales
x is the independent variable which in this case is Income
m is the slope and based on my calculations, it is 0.011
b is the constant and based on my calculations, it is -722.142
We want to predict the income which is the x hence, we need to make x the subject of the initial formula - x = (y - b) / m
x = (y - -722.142) / 0.011
 
The DAX to calculate b
 
The DAX to calculate m
●	Which customer do you predict has the highest income?
Jon Little is the customer with the highest predicted income
 
 
●	Which product will be advertised the most?
The marketing team should focus on advertising the Chronograph Watch and Leather Sneakers because they are the highest rated product with an optimal price point.
