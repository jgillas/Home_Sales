# Home_Sales

In this challenge I was asked to run multiple queries to determine different different prices for different apartments. I was also asked to change the data three times to determine which runs faster. 

The first query returns the average price, rounded to 2 decimal places for a four-bedroom house sold each year. A picture of the query is below: 

  <img width="377" alt="Screenshot 2023-08-10 at 4 20 03 AM" src="https://github.com/jgillas/Home_Sales/assets/125215083/fcd712ae-d312-4bd5-ae3a-8a15cfa0bf93">

The second query returns the average price, rounded to 2 decimal places for a home that has three bedrooms and three bathrooms. A picture of the query is below: 

  <img width="371" alt="Screenshot 2023-08-10 at 4 21 16 AM" src="https://github.com/jgillas/Home_Sales/assets/125215083/d8a22898-35a9-4882-9f50-18b6734dc915">

The third query returns the average price of a home with three bedrooms, three bathrooms, two floors, adn is greater than or equal to 2,000 square feet for each year built, rounded to two decimal places. A picture of the query is below:

  <img width="664" alt="Screenshot 2023-08-10 at 4 22 42 AM" src="https://github.com/jgillas/Home_Sales/assets/125215083/25c9a67d-d9af-4a08-b036-221e326a8dfd">

The fourth query returns the view rating for the average price for homes that are greater than or equal to $350,000, rounded to 2 decimal places. The run time is also shown for this query. A picture of the query is below:

  PIC

I then created a cache of the temporary "home_sales" table. I ran the fourth query over again with the cached temporary table and computed the run time again. A picture of the query is below: 

  PIC

I then created a partition of the home sales dataset by the "date_built" field and formatted parquet data to be read. I then created a temporary table of the parquet data. I ran the fourth query agian with the parquet data and computed the run time again. A picture of the query is below: 

  PIC

