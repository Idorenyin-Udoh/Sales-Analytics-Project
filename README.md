# PABLO STORES 2019 SALES ANALYTICS

## Table of Contents

- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [The Data](#the-data)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Data Exploration](#data-exploration)
- [Insights](#insights)
- [Recommendations](#recommendations)
- [Next Steps](#next-steps)

### Problem Statement

Pablo Stores faces challenges in its sales data management which has hindered decision making and limited the ability to capitalise on business opportunities. Some of the key issues as communicated by the CEO, Pablo include:

- Lack of an integrated view of best and worst-selling products impedes inventory optimization and targeted marketing. 
- Inadequate insights into city-wise sales prevents them from tailoring strategies to regional market variation. 
- Absence of dynamic daily and monthly sales trends hinders their ability to respond to market changes and capitalise on emerging opportunities. 
- Store outlets rely on manual and time-consuming data compilation processes, resulting in inefficiencies and errors that impedes strategic decision-making and operational efficiency. 
- Accessibility restrictions within the stores constrain the sharing of sales data, inhibiting collaboration and the development of a data-driven organizational culture. 

### Objectives

This project seeks to address these challenges by creating a user-friendly Sales Dashboard tailored for Pablo Stores, leveraging advanced data analytics and visualization tools. The envisioned dashboard aims to provide insights into product performance, geographic sales variations, and timely trends for the year 2019, fostering informed decision-making and propelling Pablo Stores towards sustainable growth. The entirety of this project will be done using Microsoft Excel. 

### The Data

The dataset for this project was provided by [Meriskill](https://www.linkedin.com/company/meriskill/). It contains 185,951 rows and 11 columns with the following information:

1. An unlabelled column numbered from 0, serving as the index for each row
2. Order ID
3. Product
4. Quantity ordered
5. Price each
6. Order date
7. Purchase address
8. Month
9. Sales
10. City
11. Hour


### Data Cleaning and Preparation

Once I downloaded and imported the data into Excel, I proceeded to clean and prepare it for analysis. Firstly, I created a new version of my data in case I needed to drop some columns or make other changes. In the newly created worksheet, the following steps were taken: 

- **Duplicate check**: I made sure to confirm that all the rows in the dataset were unique.
- **Missing values**: I did a thorough check for blanks in all the columns. There were no missing values.
- **Data types**: All columns were in the General format which is fine for what I need to do.
- **Outliers**: The majority of sales per order were below $200, resulting in a skewed distribution but that was expected. Also, most of the orders were for a single quantity of a product which is also fine.
- **2020 transactions**: Even though it was a 2019 dataset, the transactions recorded on the first day of 2020 were included. These were deleted to maintain the integrity of the dataset for the specified year.
- **Categorical variables**: I examined the categorical variables for errors in spellings and other unexpected values. Again, everything was fine.
- **Column removal**: Even though I wouldn't need some columns (like the purchase address column) for my current task, I decided to keep them for potential future analysis.
- **Data extraction**: For clearer analysis, I extracted the month and day of the week from the order date column using =TEXT(G2, “mmmm”) and =TEXT(G2, “dddd”) respectively. So, I had December instead of 12 and Monday instead of 1. I then deleted the original month column (whose values were recorded in numbers).

### Data Exploration

With the data now clean and prepared, it was time for exploration and analysis. Pablo wanted to know which products were doing well so, using a pivot table, I extracted the total quantity of products ordered/sold and filtered to get the top 5. Then I repeated the process but filtered for the bottom 5 products this time to pinpoint those with the lowest sales. 

Secondly, I looked at the geographical data. Using the same process as above, I extracted the total sales per city to know which city influenced sales the most and which didn't do too well. 

Pablo also wanted to track daily and monthly trends so I extracted the total sales per month and the average daily sales. 

To make my dashboard dynamic and get even more specific information, I created three slicers:

- A product slicer to get city sales, total monthly sales, and average daily sales specific to each product.
- A city slicer to get the quantity of products sold, total monthly sales, and average daily sales specific to each city.
- A month slicer to get the monthly distribution of quantity of products sold and city sales.

### Insights

1. **Top Products**: AAA Batteries, AA batteries, USB-C Charging Cable, Lightning Charging Cable, and Wired Headphones emerged as the top 5 best-selling products, with AAA Batteries leading at 31,012 units sold.
![Top products](https://github.com/Idorenyin-Udoh/Sales-Analytics-Project/assets/162564901/e93f53ea-30d5-4199-816a-2e91975b1340)

2. **Bottom Products**: LG Dryer, LG Washing Machine, Varebadd Phone, 20in Monitor, and ThinkPad Laptop were the top 5 worst-selling  products, with LG Dryer selling only 646 units the entire year.
![Bottom products](https://github.com/Idorenyin-Udoh/Sales-Analytics-Project/assets/162564901/d3111d04-0f7d-46a9-aedb-8f1918cf405b)

3. **Geographical Variations**: San Francisco led in sales, followed by Los Angeles, while Austin recorded the least sales.
   ![City sales](https://github.com/Idorenyin-Udoh/Sales-Analytics-Project/assets/162564901/8a85d33f-3f14-4497-80f4-3125e8f362ba)

4. **Monthly Performance**: December recorded the highest sales with over 4.6 million dollars, while January had the lowest sales with less than 2 million dollars.
   ![Monthly sales](https://github.com/Idorenyin-Udoh/Sales-Analytics-Project/assets/162564901/8c06d8fe-487e-4574-9d45-a57d82325ed6)

5. **Daily Trends**: Wednesday and Tuesday had higher average sales than other days, while Thursday was the day with the least sales activity.
   ![Daily sales](https://github.com/Idorenyin-Udoh/Sales-Analytics-Project/assets/162564901/7ca4a91f-873e-4199-85ca-ff4fa2f407f4)



### Recommendations

Following a comprehensive analysis of the sales data, the following recommendations are proposed to enhance the performance and growth of Pablo Stores:

- Pablo Stores must capitalize on the success of the top-selling products and implement targeted marketing strategies. They can use customer insights to tailor promotions and advertising, maximizing visibility and sales for these high-performing items.
- Opportunities for diversification by identifying potential substitutes or complementary products should be explored. Introducing new items that align with customer preferences can contribute to increased sales and provide a more expansive product offering.
- Opportunities for diversification by identifying potential substitutes or complementary products should be explored. Introducing new items that align with customer preferences can contribute to increased sales and provide a more expansive product offering.
- They should implement strategies to enhance customer engagement, such as loyalty programs, personalized recommendations, or exclusive offers. Building a stronger connection with customers can lead to repeat business and positive word-of-mouth marketing.
- The online presence of Pablo Stores should be expanded by investing in e-commerce capabilities. This will not only broaden the customer reach but also provide valuable data for online sales trends and customer behaviour.

### Next Steps

This section outlines a strategic plan for executing the recommendations. These next steps are designed to ensure a seamless transition from analysis to actionable results, promoting a dynamic and responsive business environment.

1. A detailed roadmap for the implementation of the recommended strategies should be developed to serve as a practical guide for the step-by-step execution of proposed initiatives.  Specific timelines, responsible parties, and key milestones for each recommendation must be outlined.
2. A comprehensive plan for monitoring and evaluating the effectiveness of implemented strategies should be established. KPIs related to sales, customer satisfaction, and other relevant metrics should be defined. Progress will be accessed against these benchmarks to ensure the ongoing success of the initiatives.
3. Staff training programs should be organised to equip staff with the necessary skills and knowledge required for successful strategy execution. Employees must be well-prepared to embrace data-driven decision-making, customer engagement techniques, and any new processes introduced.
4. Opportunities for integrating advanced data analytics tools or Customer Relationship Management (CRM) systems to streamline processes and enhance decision-making capabilities should be looked at. Potential partners should be evaluated and the integration process initiated as part of the overall strategy implementation.
5. Periodic performance reviews to assess the impact of implemented strategies should be scheduled. These reviews will be used to identify areas of success, areas for improvement, and any unforeseen challenges. The business strategy can then be adapted as needed based on the evolving business landscape.
  

