# Comprehensive-Sales-Analysis
## Understanding product performance and profitability is paramount for the success of shopping malls. With the increasing diversity of consumer preferences and the evolving nature of retail trends, it is crucial for mall management to strategically assess and optimize their offerings to drive revenue and maintain competitiveness.
Read full analysis with each image of analysis on Medium page via this Link https://medium.com/@Esther.0/understanding-customer-behavior-and-optimizing-marketing-strategies-in-istanbul-shopping-malls-bac6d6764b39

### Introduction and Objectives:

This project delves into analyzing a dataset comprising shopping information from 10 distinct shopping malls in Istanbul. I use pivot tables in Excel to explore various facets of customer behavior, including demographics, popular product categories, payment methods, shopping trends, and profitability insights. The overarching goal is to leverage these insights to optimize marketing strategies and store layouts, ultimately enhancing customer engagement and maximizing profitability for the malls.

### The primary objective of this analysis is to comprehend customer behavior and spending patterns within Istanbul’s shopping malls. By doing so, we seek to optimize marketing strategies, product offerings, and store layouts to increase customer engagement and maximize profitability. Specifically, we aim to explore the following aspects:

Customer Demographics

Product Analysis

Payment Methods

Seasonality/Trends in Spending

Profitability Analysis

Data Description:

The data utilized for this project consists of sales records from ten different shopping malls in Istanbul. It was provided in the form of a CSV file, which was converted into an Excel workbook. The dataset spans from 2021 to 2023, encompassing three years of sales records from ten different shopping malls in Istanbul, and contains detailed information for each shopping transaction.

The variables included in the dataset are as follows: transaction invoice no, customer ID, Gender, Age, Category, Quantity, Price, Payment method, Invoice date, Shopping Mall

### Data Manipulation:

To achieve the depth of analysis required for this project, several data manipulation techniques were employed:

Age Distribution Column: An additional column was created to categorize customers into age groups using a nested IF formula in Microsoft Excel. The syntax used is as follows:
=IF([@Age]<=29, "18–29", IF([@Age]<=39, "30–39",
IF([@Age]<=49, "40–49",IF([@Age]<=59, "50–59", 
IF([@Age]<=69, "60–69")))))

2. Date Formatting and Month Extraction:

The dataset contained dates in an improper format. To address this issue, the TEXT formula in Excel was employed to correctly format the date column. Additionally, a new column was added to extract the month from the formatted dates. This allowed for better organization and analysis of the data based on monthly trends.

The syntax used is:

=TEXT([@[Invoice_date]],"MMM")
3. Season Column: A new column was added to categorize transactions by season for seasonal and trend analysis. The formula used is:

  IF(OR(MONTH([@[Invoice_date]])=6, MONTH([@[Invoice_date]])=7, 
MONTH([@[Invoice_date]])=8), "Summer",
      IF(OR(MONTH([@[Invoice_date]])=9, MONTH([@[Invoice_date]])=10, 
MONTH([@[Invoice_date]])=11), "Autumn",
            IF(OR(MONTH([@[Invoice_date]])=12, MONTH([@[Invoice_date]])=1, 
MONTH([@[Invoice_date]])=2), "Winter", "N/A"))))
These data manipulation steps were essential for preparing the dataset for in-depth analysis, allowing insights into customer demographics, shopping trends, and seasonal patterns across the shopping malls.

### Methodology:

The methodology combined data cleaning, data manipulation, organization, pivot table analysis, and statistical techniques to gain a comprehensive understanding of the shopping data and extract actionable insights for optimizing marketing strategies and store layouts.

## Analysis and Findings

### Customer Demographics:

### The distribution of customers by gender across different shopping malls:


The Mall of Istanbul boasts the highest distribution of both Male and Female customers, comprising 20.05% of the total customers. This represents a 0.32% increase compared to Kanyon Mall.

Forum Istanbul has the lowest distribution of both Male and Female customers, comprising only 4.97% of the total customer base.

Across all ten shopping malls, Females make up the largest portion of the customer demographic, accounting for 59.81% of the total customer base, while Males represent 40.19% of the total customer base.

### Average Age of Customer in each Shopping Mall

From the analysis, the average age for both male and female customers is mostly consistent across all shopping malls, with an average of 43 years.

However, Zorlu Center, Emaar Square Mall, and Forum Istanbul have a slightly higher average age of 44 for both genders.

This suggests that there is generally little variation in age distribution by gender among these malls.

### How does the Age distribution vary by Gender?

The table indicates that the largest customer-based age group is 18–29, comprising 23.17% of the customer population, representing a 3.78% increase from the 30–39 age group.

Following 18–29, the subsequent largest age groups are 30–39, 40–49, 60–69, and 50–59.

In all age groups, the patronage level of female customers exceeds that of male customers.

Moreover, as age increases, there is a reduction in their patronage level. This suggests that older individuals exhibit lower rates of mall patronage compared to younger age groups.

### The significant difference in spending habits between male and female customers within each shopping mall

There is significant variation in purchasing behavior and spending habits between male and female customers across all ten shopping malls.

Female customers exhibit a higher purchase rate compared to male customers in all the shopping malls, comprising 59.81% of the total customer base, which is a slight increase of 0.20% from male customers. Conversely, male customers make up 40.19% of the total customer base.

In the Mall of Istanbul, which has the highest transaction Mall, females account for 11.97% while males account for 8.08% of the total transaction recorded.

At Kanyon Mall, females have the highest spending habits, representing 11.97% of the total transactions, compared to 7.96% for males.

### The age demographics for the top-selling product categories

The top-selling product category is Clothing, accounting for 34.68% of the total sales among the eight product categories offered by the malls.

This represents a 0.19% increase from Cosmetics, which comprises 15.18% of the total sales.

The age group contributing significantly to this increase is 18–29, representing 23.17% of the total patronage.

### Do certain age groups show a preference for specific payment methods?

The 18–29 age group leads in all payment methods — Cash, Credit Card, and Debit Card — representing 23.17% of the total transactions.

Cash remains the most preferred transaction method across all age distributions, accounting for 44.69% of the total transactions recorded.

The 18–29 age distribution exhibits a high preference for all payment methods.

Following the 18–29 age group, the 60–69 age distribution shows a notable preference for Cash payments at 8.63%, while the 50–59 age group demonstrates the lowest preference for Cash Payment but they have more preference for Debit Cards.

For Credit Card payments, the 30–39 age group follows closely after the 18–29 age group.

Both the 30–39 and 40–49 age distributions show relatively an equal preference for Debit Card payments.

## Product Analysis:

### Which product categories are the most popular across all shopping malls?

The most popular product categories across all shopping malls are Clothing, Cosmetics, and Food & Beverages. Clothing emerges as the top-selling category, accounting for the highest total sales, followed by Cosmetics and Food & Beverages. Clothing accounts for 34.67% of the total sales transactions.

Cosmetics which is the second most sought-after category after Clothing, accounts for 15.22% of the total sales across all ten shopping malls, followed by Food & Beverages, which represents 14.82% of all transactions.

### Top Selling Products in the Product Category

The top-selling product among the eight categories is Clothing, with a total quantity sold of 103,558, accounting for 34.67% of the total sales. This is followed by Cosmetics, representing 15.22% of the total quantity sold, and Food & Beverages, which represents 14.82%.

### How does the quantity of products sold vary by category and shopping mall?

The quantity of product sales varies with the category and the shopping Mall as the Quantity sold for Clothing influences the total patronage level of the Mall of Istanbul making it highly patronized among the shopping mall.

Cosmetics with Food& Beverages increases the Quantity sold at Kanyon and Metrocity.

Quantity Sold in the Clothing category has a big influence in all the malls.

The quantity of goods sold in all categories varies from Clothing being the highest taking up 20.12 of the total quantity sold in Mall of Istanbul while the Clothing category takes 34.67%.

### How does the average price per unit vary across different product categories?

The Technology category has the highest average unit price of $3,156.94, indicating that it is a high-cost product. Following closely is the Shoes category with an average price of $1,807.39.

The Food & Beverage category has the lowest average price among all the product categories.

### Are there any noticeable trends in the purchase quantity of products over time for each category?

The purchase quantity of all product categories has declined over the years. Each of the eight categories began in 2021 with moderate sales percentages, which slightly decreased in 2022.

However, Clothing experienced a minor decrease of 0.003% in 2022 as well as other product Categories.

Subsequently, there was a significant decline in 2023, with Clothing experiencing a notable decrease of 0.13% from 2022 sales. The rate at which Quantity sold in the Clothing category decreases tremendously in 2023 is the same rate at which all other category declines too.

### For each product category, what is the average number of items purchased per transaction?

Cosmetics, Shoes, Books, Technology, and Toys all have an average quantity of 3.01 items per transaction.

Clothing and Food & Beverage have a slightly lower average quantity of 3.00 items per transaction.

Souvenir has the lowest average quantity at 2.97 items per transaction.

Overall, customers tend to purchase around 3 items per transaction across most product categories, with some minor variations.

## Payment Method Analysis:

What are the preferred payment methods across different shopping malls?


The preferred payment method across all shopping malls is cash, accounting for 44.69% of total payment transactions, followed by credit cards at 35.12%.

Debit card is the least preferred payment method across all ten shopping malls accounting for just 20.19% of the total transaction.

Customers at the Mall of Istanbul predominantly prefer cash, as is the case in all other shopping malls

### Is there a correlation between payment method and purchase amount?

Yes, there appears to be a correlation between payment method and purchase amount. Customers who pay with cash tend to make higher purchases compared to those who use cards.

This can be inferred from the fact that cash transactions account for a significant portion of the total transaction amount, indicating that customers using cash are likely to spend more on their purchases.

### What is the average transaction value for each payment method?

The Average transaction value for Cash Mode of Payment is $690.82 with Credit Cards having an average transaction value of $688.54 and Debit Cards being the lowest with $687.03.

### Do certain payment methods tend to be associated with higher quantities of products purchased per transaction?

In terms of the number of products purchased per transaction, the cash payment method tends to have the highest, with 133,370 products purchased, while Debit Card transactions show the lowest quantity per transaction, at 60,297 items.

Cash payment methods often result in higher quantities of products purchased per transaction compared to debit or credit card payments.

### How has the usage of different payment methods evolved over the period?

Cash and Credit Card payments saw an increase in 2022 followed by a significant decline in 2023, while debit card payments have been declining consistently over the period.

Cash payment method increased by 0.0014% in 2022 and declined by -0.17% in 2023.

Credit Card mode of payment increased by 0.0017% in 2022 and declined by -0.13% in 2023.

Debit Card mode of payment declined by -0.0014% in 2022 and declined by -0.075% in 2023.

### Is there a correlation between customer age and preferred payment method?

There is a consistent pattern: cash is the most preferred payment method across all age groups, followed by credit cards, and then debit cards. But highly preferred among the 18–29.

## Seasonality/Trends in Spending:

### How does the total sales volume vary month-over-month and year-over-year?

In 2021, July and October are the peak Month having the highest total sales, with $2,802,468.58 and $2,782,418.40 respectively.

February has the lowest sales, with $2,358,636.34.

Total sales fluctuate throughout the year, with slight variations from month to month.

In 2022, October is the Peak month having the highest sales with a sum of $2,755,839.69, then followed by July which has a total sum of $2,749,554.99.

Relative to 2021, February shows to be the month with the lowest sales.

The sales trend in 2022 has little variation and fluctuation between months and throughout the year, the sales weren’t consistent.

In 2023, January was the peak month having the highest sales recorded, the sales dropped a little with-0.0009% in February

There was a significant fall in sales in March.

Total sales show a significant decrease in 2023 compared to the previous year. However, the analysis was conducted for just three months: January, February, and March of 2023. If the mall does not take recommended actions, the drastic fall that started in March 2023 might continue and significantly affect the mall’s sales.

### Are there any seasonal trends in the sales of specific product categories?

In all four seasons — Autumn (September, October, and November), Spring (March, April, and May), Summer (June, July, and August), and Winter (December, January, and February) — it’s interesting to note that clothing remains the most patronized product category and has the highest total sales among all eight categories. The trend in all four seasons remains constant, with clothing leading the category, followed by shoes, technology, and cosmetics.

Books and souvenirs consistently have lower sales and are not as well patronized by customers.

### Do certain shopping malls experience higher sales during specific times of the year?
From analysis, All Malls tend to enjoy higher sales in January apart from Viaport Outlet Mall and Zorlu Center which has their highest Sales in February.

January sales significantly contribute to the total sales of Mall of Istanbul, Kanyon Mall, Emaar Square Mall, Metrocity, Metropol AVM, and Cevahir AVM.

### Do certain product categories experience higher sales during specific months of the year?

Yes, from the analysis, certain product categories experience higher sales during specific months of the year.

Shoes experienced an increase in sales in May, with a rise of 0.21% from the previous month (April).

Technology also saw an increase in May, with a growth of 0.14% from the previous month.

Cosmetics increased by 0.01% in May compared to the previous month’s sales.

Toys also increased in May with a growth of 0.002% after dropping consistently from February.

Sales of Clothing, Shoes, and Technology increased in July.

Sales of Shoes increased in August.

Clothing sales increased drastically in October, as well as sales of Shoes and Technology but not as high as January and February sales.

May sees an increase in sales for shoes, technology, cosmetics, and toys, while July experiences an increase in sales for clothing, shoes, and technology.

### How has the total sales volume changed from year to year across all shopping malls?

Total sales recorded started from 2021 having 45.68% of total Sales, In 2022, it increased to 45.68% of total sales, and sales drastically dropped in 2023 to 8.55% of total Sales.

The product category that contributed to the Sales trend.

Clothing contributed highly to the sales trend followed by Shoes, Technology and Cosmetics.

Books and Souvenirs contributed the least to the sales trend.

## Profitability Analysis

Which product categories generate the highest revenue and profit margins?

From the analysis, Technology generates the highest revenue and profit Margin, followed by Shoes, Clothing, and Cosmetics.

Food& beverages are highly patronized but do not generate more revenue and as well profit.

### Patronage level and profit Margin
Technology shows a high-profit Margin despite its low patronage with $3,156.94 being the highest average price among all product categories.

Follows by Shoes, despite not being so high patronage product compared to the Clothing category, Shoes has the second highest average price of $3,156.94 as well as profit margin.

Food & Beverages are relatively one of the high-selling products but have the lowest profit margin among product categories. On the other hand, Technology, despite being a low-selling product, has the highest profit margin.

Clothing is the highest-selling product, but it doesn’t yield the highest profit margin for the Mall.

Shoes are a moderately selling product but have a good profit margin.

### The Mall that produces a higher Profit Margin

Emaar Square Mall has been constantly demonstrating higher profitability than all other malls.

### Underperforming Product Category
From the analysis, there are a few categories that seem to consistently underperform across multiple shopping malls:

Cosmetics: It has low sales and return on profit in both Metropol AVM and Metrocity.

Toys: It has the lowest sales and return on profit in Forum Istanbul.

Books: It has the lowest sales and return on profit in Viaport Outlet.

Souvenirs: It has the lowest sales and return on profit in Zorlu Center.

## Recommendations:

Targeted Promotions:
Tailor promotions and discounts to appeal to specific age groups. For example, offer discounts on technology products for younger customers, 18–29 and 30–39 Age distribution, and special promotions on luxury items for older customers, Aged 40 and above

Introduce a bundled sale where customers are encouraged to purchase more than one item. For example, offer a promotion where the purchase of clothes, shoes, and cosmetics together entitles the customer to a free product. Alternatively, offer a discount when customers buy items from three different categories.

Omni-Channel Marketing:
Implement an omni-channel marketing approach to cater to different payment preferences. Offer online payment options for customers who prefer credit or debit cards with no charges to be debited from the bank account from the Supermarket and in-store promotions for those who prefer cash. The Mall management should remove any restriction input on Credit card and Debit card payments to encourage customers to purchase as many products as they want with their cards both Debit and Credit Cards, if possible at no interest rate.

Cash flow is vital in any business, so mall management should incentivize cash payments by offering discounts to customers who spend a certain amount on goods per transaction.

Seasonal Campaigns:
The Management should develop seasonal marketing campaigns that align with customer preferences and shopping trends. For example, promote outdoor gear and sporting goods during the summer months and focus on cozy apparel and home goods during the winter.

Customer Loyalty Programs:
Launch customer loyalty programs to incentivize repeat purchases and foster customer loyalty. Offer exclusive perks, discounts, and rewards based on purchase behavior and membership levels. Customer loyalty Cards drive existing customers to patronize more and introduce more customers to the Mall.

### Conclusion

In conclusion, the analysis of shopping data from ten different malls in Istanbul has provided valuable insights into customer behavior, product performance, payment method analysis, and marketing opportunities. Here are the key findings:

Customer Demographics: The analysis revealed variations in customer demographics across different age groups, with each group exhibiting different shopping preferences and spending habits.

Product Performance: Certain product categories, such as technology having a lower patronage level but remaining the high-earning product category, clothing, cosmetics, and shoes, consistently performed well across all malls, while others, like Books, Souvenirs, and toys, showed lower sales and profitability.

Payment Methods: There were notable differences in preferred payment methods among customers, with some preferring cash, while others favored credit or debit cards.

Seasonality and Trends: Seasonal trends in spending habits were observed, with sales performance over the year and monthly trends.


