CREATING A COMPREHENSIVE EXPLORATORY DATA ANALYSIS (EDA) REPORT FOR GLOBAL ELECTRONICS
OBJECTIVE 
To uncover insights into customer demographics, purchasing behaviours, product performance, store operations, and the impact of currency fluctuations on sales. 
Highlight the ultimate goal of leveraging these insights to inform marketing strategies, inventory management, sales forecasting, product development, and store operations.
DATA CLEANING 
 1. Handling missing values

        Sales Dataset
            a)	Dropped ‘Delivery_Date’ column since 79% of the data were missing     
        Stores Dataset
            a)	‘Square Meters‘ column has one missing value for ‘online’ stores, for which     having ‘Square Meters’ doesn’t makes sense so replaced it with ‘0’         
        Customers Dataset     
            a)	The column ‘State Code’ having ‘NA’ as State code for the state ‘Napoli’ Which was mistaken as ‘Nan’ while reading the csv file into the jupyter notebook
            
            b)	Thus imputed the null values with string “NA”  

 2. DATATYPE COVERSIONS
            Sales Dataset
            	Converted ‘Order_date’ column to date format
            Stores Dataset
            Converted ‘Open_date’ column to date format
            Customers Dataset  
            	Calculated ‘Age’ column from birthday column
            Product dataset
            	Converted Unit_Cost_USD and Unit_Price_USD to numeric
3. LOADING DATA
           After completing data cleaning I load the tables into SQL from jupyter notebook
5. CREATED INTERACTIVE DASHBOARDS USING POWER BI 
            Connecting SQL with power bi , created different sql query to do different visualizations to gain insights from the tables
6.KEY INSIGHTS         
       1. CUSTOMER DEMOGRAPHICS  
            
            i.	Gender is normally distributed     
            
            ii.	Age is also slightly normally distributed with people above the age 59 being the major contributor (44%) to the sales  
                 
            iii.	Customers from United States are the major group and from France are the minimal group 
       2. PURCHASING PATTERN      
            i.	There is a upward trend on the sales till 2019 (2016,2017,2018) then there’s a drastic drop in sales from 2019 to 2021   
             
            ii.	The average amount of money spent per order by all age groups monthly over the years is around 850 USD
            
            iii. On an average the purchase frequency of customers for every year is 1
            iv.	The country United states is the major contributor to the revenue 
       3. PRODUCT PERFORMANCE
            i.	Categories such as Computers and Home appliances are the major contributors to the revenue
            
            ii.	Sub-categories such as Desktops are the major contributor to the revenue. 
                Sub-categories such as Televisions, Projectors & Screens, Water Heaters, Camcorders, Laptops, Movie DVD, Touch Screen Phones are the second major contributor to the revenue. 
            
            iii.	Popular products in terms of quantity sold and total sales are 
                    a)	WWI Desktop PC2.33 X2330 (Black)
                    b)	Adventure Works Desktop PC2.33 XD233 (Silver)
                    c)	Adventure Works Desktop PC2.30 MD230 (White, Black,  Silver)
                    d)	Adventure Works Desktop PC1.80 ED180 (Black, Silver, White )
                    e)	Adventure Works Desktop PC1.60 ED160 (Black, White)
                    f)	WWI Desktop PC1.80 E1801 (Black)
                    g)	WWI Desktop PC1.80 E1800 (White)
                    h)	WWI Desktop PC1.60 E1600 (Black, Silver, Red)
       4. STORE OPERATIONS
            i.	Store in United States with square meters 2000 and Online stores are the high performing stores in terms of revenue earned 
            ii.	Australia with square meters (2000) has decent performance whereas Australia with square meters (665,595) is under-performing 
            iii.	France is the least performing stores compared to other stores also having square meters less than 500
            
                        

7. ACTIONABLE RECOMMENDATIONS AND MARKETING STRATEGIES
        a) To increase Frequent purchase 
        •	Reward customers with discounts,reward points
        •	Create personalized offers and communications for high valued customers
        •	SMS and Email Marketing
        b) Inventory Management
        •	Optimize stock levels for top-selling products especially for Stores in United states, United Kingdom
        c) Store Expansion
        •	Expand the stores in United states and Australia to 2000 square meters
        d) Increase average order value
        •	Bundle products that are popular
        •	Create Free shipping and other gifts for high valued customers


