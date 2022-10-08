Please read me for all the important information about this repository.

This code examines and analyzes data on if drivers will accept a coupon.


In this Jupityer notebook we are examining data about the use of coupons by drivers.  The dataset contains information ranging from the age,income, employment, and marital status to how often the driver frequents different types of establishments and how far away a coupon establishment is from the driver currently.  With this information we are trying to determine if the driver will accept and use a certain type of coupon.

Once the dataset was loaded did a preliminary examination to see if any correlations stood out, examine if there were any columns with missing values that needed to be addressed, and anything else about the data that stood out.  The findings were that no numerical data appeared to have any strong correlations, there were a few columns with missing data that needed to be addressed, and a few other notables.  The other notables included combining the direction data into one column and creating a new column to clearly state if the drivers accepted the coupon.

Addressing the missing data was a bit more complex.  The car column had so much missing data it was simply dropped.  The Bar data was examined to see what was the most common value and it was noted that a large majority never went to bar or went less than once.  The decision was made to fill the values with less than 1.
The Coffeehouse data was more uniformally distributed thus the decision was made to fill the missing data with the most common value, also 'less1'. The other data was currently left as null until if/when it would be explored further.

The analysis of the data then began.  We began by simply looking at the total number of drivers that accepted the coupon and found 57% of drivers accepted the coupon they were given. We then took a look at what the acceptance was based on the coupon provided.  We saw that cheaper restaurants and carry out/take away had the highest accpetance rate while Bars and expensive restaurants had the lowest rates.  This would seem to make logical sense as most drivers and people overall are apt to visit cheaper restaurants and/or carry out meals, while fewer people overall are likely to go to bars and/or visit expensive restaurants.

In the next section we took a more in depth look at the Bar coupon data. We began by creating a new dataframe



