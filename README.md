# Healthcare Predictions
## Making a difference for heart disease patients

**Author**: Justin Faber

### Objective:

What key metrics best predict heart disease? By knowing only a few key things about patients, can we predict their future health? Time to find out! 


### Data:
We have, in total, just under 1,000 patients and their health information. Some of our key metrics include the patient's age, sex, cholesterol, their resting blood pressure and their max heartrate. In total we have 11 key metrics per patient, to help us evaluate the all important 12th variable: do they have heart disease?


## Methods
- To prepare our data for this project we did the following:
  - Removed any duplicate rows from within our dataset
  - Explored any missing values from within our data
    -  While we noticed that there weren't any actual "missing values" in our data, we did find an occurance of "0" for one patient for their resting blood-pressure. This certainly isn't possible, so we treated this value the same as "missing", and with only a single row being affected we just dropped that one row. 
  -  We looked for any potential outliers from within our dataset, but found nothing so far outside of the norm that warranted removal, so we left all remaining data in the dataset for further exploration!

## Results
Our first goal was to better understand our data, and look for strong correlations between any of the features and our target. After a deep dive into all of the different featues, we came out with two major takeaways and two major correlations. Each expressed and explained in the following visualizations:


#### Heart Disease Prevelance By Exercise Induced Angina
![VIZ 1](Heart_Disease_Visual_1.png)

> What we're learning so far is that total sales by outlet type is pretty similar across our different outlet types! Every category is a close race, regardless of which type of outlet we're looking at. But also noticable, is that each outlet type has a slightly better area than the rest. Grocery stores outsell everyone else in Fruits & Vegetables, while Supermarket Type 3 gets the nod for Household Goods, and Supermarket Type 1 wins by a hair in the Snack Foods department. 

#### Total Sales By Outlet
![VIZ 2](Heart_Disease_Visual_2.png)

> Our entire dataset is comprised of sales from 10 different unique outlet locations. In looking at total sales for each of them individually, we can see that they are all extremely close! Every outlet that we have shows sales beteen 8.5M and 10M total. Between our first visualization and this one, it's easy to see that simply looking at categories of sales and which outlets they belong to, isn't going to be enough to help us predict sales moving foward. That's OK though, it's not supposed to be easy! This is where machine learning can help! It can find correlations and connections in our data that may not seem intuitive for us initially. Let's make some models! 

## Model

After exploring and testing multiple models, our highest performing model for our data was a random forest model

This final model had an RMSE of 1,076.12 and an R^2 of 59.76%

While not "perfect" by any stretch of the imagniation, this model can still provide some valuable insight into our sales, as it accounts for nearly 60% of the sales variance in our data. 

## Recommendations:

We need to continue to gather more data to help the model. While we can use the model to provide us some insight for future decisions, an R^2 of just below 60% can be improved upon. We need to make it a point to gather as much data as we can in the coming months to feed our model more information. With more information we should be able to further improve the accuracy of our model and get to an R^2 number that we can all be comfortable with! 



### For further information


For any additional questions, please contact **JFaberSFSD@gmail.com**
