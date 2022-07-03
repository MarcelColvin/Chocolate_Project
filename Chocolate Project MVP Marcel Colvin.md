## Chocolate Project MVP

**Opportunity**:
We are interested in finding out what factors make a good chocolate bar and optimizing the factors for cost. This will allow us to find how to make the best chocolate bar for the cheapest cost.

**Impact Hypothesis**:
We hypothesize that there will be factors and ingredients that have an impact on the rating of a chocolate bar, which we can then use along with cost data to find the cheapest way to make the highest rated chocolate bar.

**Solution**:
The solution path planned out here is
1.	Find consequential factors in a model that impact the rating
2.	Combine these factors with their cost
3.	Optimize finding the cost of the ingredients with the rating

**Data**:
The data we are working with currently is this decades long chocolate rating database. Where the Brelinkski’s have been working on rating over 2500 different chocolate bars in a database. They have provided some basic ingredients, percent cacao, and other interesting data points along with a rating. The goal is to use this data to find the most important features that make a chocolate bar achieve a high rating and how to reduce costs.

**EDA**:
The preliminary data analysis finds that the ratings are mostly centered around the average, which is making it hard to find factors that influence the rating. Taming the categorical data is a difficult process and there is only 1 continuous variable in this data set. There is one section that I have not experimented with, which is the most memorable characteristics, I am thinking of doing a VADER sentiment analysis or some other type of NLP modeling in order to get something out of this section that could impact my rating. I am also going to attempt to get Latitude and Longitude data for the company location and bean origin location to help my model.

**Modeling**:
So far in this project the current models are not performing well, but with some tuning I am optimistic that I will be able to create a model that can create a better result. The main issue is the number of multi-dimensional categorical data, most of which have almost 0 impact on the final model. There is also a lack of continuous variables, which is leading to issues with my regression models. There are still some actionable insights that I can get from these regression models, and using these combined with price data will be able to find whether we can cheaply create a tasty chocolate bar.
