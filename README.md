The tableau file is converted from live to extract in order to publish it in the public tableau platform. The link of published tableau file above:
https://public.tableau.com/app/profile/irem.anter/viz/VSTT-A1/SuperstoreAnalysis?publish=yes

The US Superstore dataset, which is obtained from Kaggle with a title “Superstore Analysis”, includes twenty-one attributes, which are as follows:

- Row ID: A unique key for each sale.
- Order ID: The ID that represents each order.
- Order Date: The date when the product was ordered.
- Ship Date: The shipping date after the order was placed.
- Ship Mode: Shipping options such as First Class, Same Day, Second Class, and Standard Class.
- Customer ID: The ID that represents each customer.
- Customer Name: The name of the customer.
- Segment: The customer segment, which can be Consumer, Corporate, or Home Office.
- Country: The country where the order was placed (United States).
- Sales: The total sales amount.
- Quantity: The total quantity of items sold.
- Discount: The discount percentage applied to the sale.
- Profit: The profit amount; if it is negative, it represents a loss.
- City: The city where the customer is located.
- State: The state where the customer is located.
- Postal Code: The postal code of the customer's location.
- Region: The region of the customer's location (West, East, South, or North).
- Product ID: The ID that represents each product.
- Category: The product category, which includes Office Supplies, Furniture, and Technology.
- Sub-Category: The product sub-category, such as Binders, Paper, Art, etc.
- Product Name: The name of the product.

In addition to the current attributes, calculated fields, sets, parameters, dynamic measures, and filters have been created using relevant formulas by using Tableau. The additional attributes are described in detail below:

- Loss?: Indicates negative profit.
- Discount: Specifies whether a discount was applied or not.
- Total Sales by State: The sum of sales amounts for each state.
  
- State Contribution Group: Groups states based on sales amount:

- Group 1: Sales amount greater than 100.000.
- Group 2: Sales amount between 50.000 and 100.000.
- Group 3: Sales amount less than 50.000.
  
- Measure Dynamic: Allows the user to dynamically switch the metric on the chart by choosing profit or sales.
- Sales per Distinct Customer: The total sales amount for each customer.
- Top 10 Products: The set, which lists the top 10 products which are ranked by sales amount.
- State Loss Amount: The total loss amount for each state.

**Dashboard 1: CUSTOMER SEGMENT ANALYSIS**

In the first pie chart, State Contribution of Sales and % of Total Profit, each color shows details about the State Contribution Group. While Group 1 represents the highest sales, the medium sales amount belongs to Group 2, and Group 3 contains the lowest sales amount. Group 3, which has the lowest sales, generates more profit than Group 2, which has medium sales. Moreover, Group 1, where states with high amounts of sales, has the highest profit rate. Focusing on campaign strategies for Group 3 might have a positive impact on the total profit.

In the second pie chart, % of Total Profit Across Customer Segments, each color shows details about the customer segments, which are Home Office, Consumer, and Corporate. While the Consumer segment has the highest impact on the total profit, the Home Office segment has the lowest impact on the total profit. Here, different kinds of strategies can be applied, such as making the Home Office segment more profitable by restricting discounts or promoting sales, or focusing on the Corporate segment to increase its profit.

In the first line chart, Sales Amount Based on the Customer Segments, seasonal trends are noticeable across the years for all segments, with end of year sales likely contributing to this pattern. Additionally, the gap between the Consumer segment and the other segments widens.

The second line chart, Seasonality in Sales for the Consumer Segment, which focuses on the Consumer segment, shows a peak in sales every September, followed by a significant drop in October. This decline can be attributed to a reduction in discounts during October. A targeted discount campaign could be introduced in September to capitalize on the peak, while strategies should be developed to address the October decline and decrease its impact.

**Dashboard 2: STATE ANALYSIS**

In the map, Sales Amount Across the States, colors represent details about the state, while the size indicates the sum of sales amount. The marks are labeled by the sum of sales. The map shows that California dominates the other states in terms of sales amount.

In the bar chart, Sales Amount & Profit Across the States, colors shows details about profit or sum of sales amount by selecting the measure names. First of all the dynamic measure has been created and added to the plot.

Lastly, the scatter plot, Avg. of Discount & Loss Amount Across the States, shows details about states. It is observed that a discount of more than 31% causes a significant loss. Ohio, Pennsylvania, Texas and Illinois with average discount rates 0.32, 0.33, 0.37, and 0.39 respectively, causes loss rather than profit. Therefore, campaign strategies should be updated and high discount rates could be eliminated for the future sales.

**Dashboard 3: REGION & PRODUCT ANALYSIS**

The first bar chart, Relationship Between Discount & Profit Across the Regions, shows the profit for each region: Central, East, South, and West. The colors indicate details about discounts. While blue represents discounted sales and orange represents sales without discounts. The chart reveals that discounts lead to profit only in the Western region, whereas other regions experience losses when discounts are applied. It would be logical to continue running discount campaigns in the Western region, because the chart demonstrates a significant profit associated with discounts in the West.

The second bar chart, Top 10 Products Based on Sales Amount, displays the total sales amount for each product, with the contribution of each region represented by different colors. A set named Top 10 Products was created to select the top 10 products ranked by sales amount. This set was then applied as a filter to generate the bar chart. According to the bar chart, the highest sales amount belongs to the product named Canon imageCLASS 2200 Advanced Copier and the Eastern region contributed the most to these sales.

In the third bar chart, Dual Axis Between Sales and Quantity for Each Region, the color indicates details about Sales and Quantity. The metrics for sales amount and the quantity sold shows similar patterns across the four regions: Central, East, South, and West. While the highest sales amount and quantity sold are observed in the Western region, the lowest levels of these metrics are seen in the Southern region.

In the scatter plot, Sum of Quantity Sold vs. Sum of Sales Amount, color shows details about sub-category of the products. While the highest amount of sales occur in Phones, the highest quantity sold occurs in Binders. While the cost of Copiers can be decreased, Binders' cost can be increased. Additionally, the cost of art can also be increased.

The last bar chart, Product Category Wise %YoY Growth, color shows details about the category of the products. The furniture category had consistent growth, with a peak in 2016 (16.65%) but slower growth in 2017 (8.29%). The Office Supplies category experienced major declines in 2014 and 2015, followed by strong recoveries in 2016 (34.03%) and 2017 (33.79%). The technology category experienced a sharp decline in 2014 and 2015, but recovered significantly in 2016 (39.06%) and this increase slowed down in 2017 (20.04%).
