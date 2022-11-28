Please read me for all the important information about this repository.

Business Understanding:

Used cars are a big business and many factors go in to what makes one used car more or less valuable than other used cars.  In order to maximize profits a used car dealership will need to have an inventory of cars with desired features at a competitive price.  Therefore, it is imperative that the used car dealership has the appropriate data and projections to be able to create adequate inventory with the competitive prices.



Data Understanding:

The first step is to look at the dataset and see what can be gleaned.  The dataset being used contains detailed information about hundreds of thousands of used car sales. From this dataset we can begin to ask some important questions to help us better understand the data.
Questions to answer:
Are there features that have a strong correlation  or no correlation with price?
Unfortunately the data has few ‘continuous’ values to begin with. This will be addressed below.  With the only continuous values being id, price, year, and odometer reading very little was gleaned. With that said there appears to be little correlation with id and a relatively strong correlation with odometer and the year.
Are there features with exclusively one particular value?
Title_status is almost exclusively ‘clean’. Possibly drop this column since it likely can’t provide meaning.
Are there features with missing values?
Some columns have many missing values and these will need to be addressed on a case by case basis.  In some cases if there are not many missing values they might be dropped from the dataset.  
Are there categorical features that need to be encoded?
This dataset has many categorical features; some of them will need to be one-hot encoded(ie Fuel), while other might be converted to ordinal values(ie Condition). Some of the categorical features with many different values might have to be addressed in a more unique way on a case by case basis.



Evaluation:
Modeling was a bit more challenging than expected.  Since a few of the columns lended themselves to one hot encoding it created a dataframe with far too many columns than was able to be processed with a home laptop.  With this restriction in mind a dataframe that was limited to 20 columns with several of the columns labeled in a less than ideal manner. The modeling produced inconsistent results as the errors were rather large. Overall, it was apparent that the features that had the most positive  impact on price was the lower odometer readings, newer cars, and more cylinders.   Some other features seemed to also play a part.  While I could certainly recommend that automatic transmissions are recommended and preferred by buyers over other transmissions, I would not feel overly confident providing any other valuable insights with the data collected and analyzed thus far. I would recommend collecting more data that correlated more with price.  As we’ve seen from previous studies it might be possible to collect data on horsepower, fuel efficiency, or other metrics that might be  correlated better with price. Another fault of this whole process is that it’s unclear which types of cars provide the most profit vs. just which cars sell for the most.  This would be essential in making suggestions to used car dealers.  It might be possible that cheaper cars sell more frequently and provide more profit but it is hard to make that conclusion from the current data.

Deployment:
Upon collecting, organizing, and analyzing the data provided in order to give insight into how to maximize profits with the sale of used cars we can provide some insight but would also feel more comfortable collecting more data and providing further analysis. Most essentially, it would be very helpful to know the profits made on previous car sales. This could be found by keeping track of the price paid for the used cars by the dealers.
But, with the data currently accessible a few things are clear:
Used car buyers pay more for cars that are newer and thus have lower odometer readings.  
Used car buyers pay more for cars with automatic transmissions. Be very wary in using inventory with other types of transmissions.
Used car buyers will pay more for electric and hybrid vehicles thus it is recommended to have these types of vehicles available for purchase.
While other factors certainly contribute to the overall price and customer interest these variables vary wildly and it can not be fully ascertained at this time as to which factors would ultimately be influential in more profits.
It is therefore recommended that we continue collecting data on what other features of used cars would contribute to customer interest and thus more profits.  With that data we can likely create better models to predict what the future may hold.







