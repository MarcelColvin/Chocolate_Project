Abstract

The initial goal of this project was to create the best chocolate bar for the cheapest amount of money. After finding a robust data set of chocolate bar ratings, but with no access to commodity pricing data, since we are in an academic setting, I pivoted the project to just finding what attributes are important in making a highly rated chocolate bar. I used google sheets and pandas to work with my data and create a model and tableau to create visualizations. The model that ended up having the most value was an optimized random forest regression, although the findings were not very significant.

Design

The initial project design stemmed from finding what attributes make a great chocolate bar and then optimizing the pricing to make the best chocolate bar for the cheapest amount of money. The [data set](https://flavorsofcacao.com/chocolate_database.html) that was found had great reviews and a plethora of data, but I was not able to combine it with a pricing data set. Therefore I pivoted into finding what attributes of a chocolate bar correspond with a high rating. This ended up being more subjective, since the rating is done by a single person over the past 10 years, but the models were useful in making some conclusions.

Data

The data set contains 2,501 rows with attributes such as Company, Cocoa Percentage, Country of Bean Origin, and Number of Ingredients. The main issue with this data was the lack of continuous numerical attributes, and the overwhelming amount of categorical data. I was also able to get Latitude and Longitude data for the Country of Bean origin to see if that was able to improve our models. The data was cleaned and converted into binary dummy variables for modeling.

Tools

Google Sheets for initial data visualizations
Pandas and Scikit-learn for data wrangling and modeling
Tableau for interactive visualizations

Algorithms

Linear Regression, Random Forest Regression and Extra Trees Regression were all experimented with before settling on Random Forest Regression as the model with the strongest performance. Random Forest Regression was used to make the conclusions about which attributes had the strongest correlation with the higher ratings of the chocolate bars.

The final model had a training set score of 0.40 and a test score of 0.09 after tuning with a Grid Search. The most important attributes that correlated with a high rating were Cocoa Percent, Vanilla, The Manufacturer Soma, a Blend of beans, a few more manufacturers, beans from Peru, and beans from Venezuela. Adding in the manufacturers was able to help the model because it seems like the manufacturers that he rates more chocolate bars from have a higher impact on the models and are more significant, such as Soma, which had over 30 ratings. The main caveat with these conclusions are that firstly the model is not very good and secondly it is not finding the attributes that make the best chocolate bar, but the attributes that influence one man's opinion about chocolate.

Communications

The google sheets document is found [here](https://docs.google.com/spreadsheets/d/1zoRUsqZVM-aiYFGaDE3YpRVj4smnRd7V7R-X-RqfudI/edit?usp=sharing), the Tableau visualizations are found [here](https://public.tableau.com/views/ChocolateProject_16568938949490/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link), and the slides are in the github repo as a PDF. The code used is found in the file Chocolate model Experimentation.ipynb
