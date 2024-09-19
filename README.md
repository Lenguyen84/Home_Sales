Home_Sales

1.Project Overview
    The goal of this exercise is to leverage SparkSQL to analyze key metrics from home sales data. We will utilize temporary views, caching, and partitioning to assess the performance of query processing times.

2.Dataset Overview
    The dataset used for this exercise can be found here: Home Sales Data. It includes property-level details such as identification, sale date, year built, price, number of bedrooms and bathrooms, living space square footage, lot size, number of floors, waterfront view, and the number of views

3.Results and Analysis:
(a) What is the average price for a four-bedroom house sold for each year?
    ![a](<Output/4 Bedroom house sold.png>)

(b) What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms?
    ![b](<Output/3Bedroom house sold.png>)

(c) What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?
        ![c](<Output/3Bedroom house_2floor.png>)

(d) What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000?
        ![d](<Output/view rating.png>)

The processing times for the SQL query related to question (d) were measured following caching and partitioning. According to the .ipynb file, the initial query took approximately 0.896 seconds. After implementing caching, the processing time decreased to about 0.579 seconds. On the second execution, the time increased to about 0.97 seconds, indicating that the cached data was evicted from memory due to memory constraints or other operations, the query would have to re-read from disk, resulting in increased execution time.

4.Instructions for Engaging with the Project:
    Due to challenges with Hadoop software on the local machine, the code for this exercise is set up to run in Colab and is stored in a file named "Home_Sales_code_colab.ipynb" within the main folder

 The dataset can be found in the main folder as "home_sales_revised.csv" and is also accessible online at the link provided in Section 2 above.

5.Citations:
    Xpert Learning Assistant
