# NYC-Airbnb-Data-Analysis

Special Notice: <br />
Because the github performs a static render of the notebooks, plotly charts can not be displayed by github. You can see the visualization script in the links below: <br />
https://nbviewer.jupyter.org/github/ChuxinYang/NYC-Airbnb-Data-Analysis/blob/master/Data%20Visualization%20Script.ipynb
<br /> <br />
Data Analysis and Visualization: <br />
We downloaded the New York City Airbnb Dataset from Kaggle Platform. This is a very rich dataset with many columns to visualize, but not enough columns for price forecasting. <br />
First, we identified the top 10 hosts with most listings and visualized their hosted locations in a map using latitude and longitude data. We found that the top host has 327 listings and Manhattan region is the preferable choice for top hosts. <br />
After that, we analyzed the listings by boroughs and neighbourhoods. Specifically, we plotted counts in pie chart and found that Manhattan and Brooklyn counts for most of the listings. Besides, we visualized price differences in violin chart and density plot. We could see that Manhattan is the most expensive region, while Bronx is the least expensive region. <br /> 
Then we analyzed the room types by plotting histograms and density plot. We found that the 'entire room/apt' is the most expensive, while the 'shared room' is the least expensive. 
<br /> <br />
Price Forecasting: <br />
For data preprocessing, we dealt with the missing values, and one-hot encoded the categorical variables. We deleted unmeaningful or unethical columns for prediction, such as ID and host_name. We made full use of the rest of the columns. For text mining, we tokenized the 'name' column based on Bag-of-Words. Finally, we split the data into train dataset (90%) and test dataset (10%). <br />
Then I built three regression models, that are Multiple Linear Regression Model, Random Forest Model, and Gradient Boosting Model. The Gradient Boosting Model emerged as the best model with 62.54% score. The result will be much better if we have more information about the properties, including number of bedrooms, house area in square feet, floor numbers, the year it was built, etc.
