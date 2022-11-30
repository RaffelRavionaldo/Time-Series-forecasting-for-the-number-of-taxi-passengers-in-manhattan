# Time-Series-forecasting-for-the-number-of-taxi-passengers-in-manhattan

To assist the operation team of the NYC Taxi commission in Manhattan to optimize the distribution of the taxi fleet

# How to Run the code :
1. Download the code (Contact me if you want the token to download via linkedin)
2. Install the requirement with this synta : pip install -r requirement.txt
3. Run the ipynb file in jupyter notebook

# Analyze

Business Problems : Operation team of the NYC taxi commission want to optimize the distribution of the taxi fleet in 1 month ahead to maximize the revenue.

To solve that problem, I make a time series forecasting model using prophet library. now let's see the dataset

![image](https://user-images.githubusercontent.com/94748637/204725977-1937f571-41fd-4ce8-bd46-6fdb85a1dcc6.png)

Dataset have 19 columns with 4 columns have null value, but the columns that have null data is not important in our analysis, so we dont need to do anything from that columns.

Now let's make a timeseries model
1. Prepare the data so that it is ready to be used to create a mode
 - Take a important columns that you need, in this case we need pickup datetime and location and order quantity. (in my code the data was in variable called final)

![image](https://user-images.githubusercontent.com/94748637/204727257-837cdb15-4b1b-40bf-900b-ef023a55dff1.png)

2. Choose one location that you want to analyze (in my case I Choose location with ID 4)
3. Make a time series model

![image](https://user-images.githubusercontent.com/94748637/204727546-8def7d3c-cb35-4d04-aa13-7eb363d2e4e7.png)

4. Make a prediction

![image](https://user-images.githubusercontent.com/94748637/204727611-99cd6875-6832-44e0-920b-3366f3374198.png)

5. Last, Analyze data from prediction

![image](https://user-images.githubusercontent.com/94748637/204727802-429afc4f-2ce1-43d1-8ae8-8ea50a79a28f.png)

From the data above, we can recommend to Operation team of the NYC taxi commission to send about 15-20 taxis between 23:00 to 03:00 everyday and besides these hours it is enough to prepare 10-12 taxis
