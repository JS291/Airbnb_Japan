# Airbnb Japan
An exploratory data analysis into the listings of Airbnb in Tokyo, Japan.

## Data
The dataset was obtained from Airbnb. - [Link](http://insideairbnb.com/get-the-data/)

Data dictionary of the columns provided by Airbnb. - [Link](https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/edit#gid=1322284596)

## Tools and Libraries
Exploration, data cleaning, and visualizations was done using Python (JupyterLab)

Libraries used: Pandas, Matplotlib, Seaborn, Numpy


# Table of Contents
1. [Introduction](#introduction) 
2. [Data Cleaning](#data-cleaning-process) 
3. [Initial Exploration](#initial-exploration)
4. [Factors to consider](#factors-to-consider)
    + [Pricing](#pricing)
    + [Ratings](#ratings)
    + [Host](#host)
5. [Areas for further exploration](#further-exploration)


# Introduction
We explore the listings in Tokyo, Japan to plan our trip.
Factors we will consider when booking a place include prices, ratings, and the host.
Through these factors we can see the quality of listings and gain better insight when planning.
Our goal is to find places that will deliver on multiple features and provide a good experience.


# Data Cleaning Process
When cleaning this dataset, I first excluded the columns of data that wouldn't be using (such as host response time and license).
Some columns were renamed so they have better readability.
Rows that contained nulls values in review score categories were dropped.
Due to the price column being displayed in local currency(Japanese Yen ¥), it was transformed to display in USD($)
Some values in columns such as price and accommodates contained the value 0 which doesn't make sense so we excluded those values.


# Initial Exploration
When we plot the listings on a map using Tableau, we notice that some areas had low concentration of listings and were in more remote regions.
As such we limited our dataset to the greater metropolitan area of Tokyo and only included neighborhoods that have 20 or more listings.
This would allow for greater access to a large variety of transportation methods.
![neighborhood_map](https://user-images.githubusercontent.com/111064486/214456311-3409ef6e-97ba-4ebe-ba5e-b991db7e434b.png)




# Factors to consider
Whenever you buy something, you want to be confident in what you are buying. Some things you would think about before making the purchase are the quality of the product, durability, and reviews from others that bought it. Booking a Airbnb or hotel room is no different, so some factors you might consider are pricing, ratings, and the host. 


## Pricing
When traveling you would have to budget for various expenses such as food, transportation cost, souvenirs, and lodging.
As we dive in the analysis in regards to pricing, we notice there are some large outliers in our listings.
To remain budget friendly, we narrow our listings and set a budget of no more than $150 per night.


## Ratings
There are 7 categories that users use to rate their quality and experience at their place of stay.
![rating](https://user-images.githubusercontent.com/111064486/214456200-cac5baf6-32b1-4be4-86d1-8714a16087cf.png)


## Host
Hosts can make or break an experience.
You want someone who is experienced, consistent, and knows how to deliver on high standards. <br><br>
We explore and compare host through various metrics such as:<br>
+ How long have they been a host?
+ Are they a superhost?
+ How many total listings do they have?
+ How many reviews do they have? Do they deliver across all rating categories?
+ What is the average and median price across all their listings?


## Further exploration
Topics to explore with other columns of data in the dataset
+ Effects of seasonality on travel/bookings
+ Which months are busiest?
+ Which neighborhoods are popular among travelers?
+ Popularity of neighborhoods based on proximity to points of interest
+ Considerations of price in regards to # of bedrooms and bathrooms when booking for a group



