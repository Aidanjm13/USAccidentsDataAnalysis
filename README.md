# US Accidents Data Analysis
### Aidan Mathieu, David Appel, Kendra Daly, Samuel Owens, Trey Kollitides
### Link to github.io static page: https://aidanjm13.github.io/USAccidentsDataAnalysis/

The goal of this project is to do exploratory data analysis on the severity of traffic accidents to determine what features cause more severe accidents. The information derived from this project could then be used to inform government officials on how to better design driving architecture or drivers on what habits they should avoid when planning to drive.

## How to Run this code

https://colab.research.google.com/github/Aidanjm13/USAccidentsDataAnalysis/blob/main/USAccidentsDataAnalysis.ipynb

This project can be inspected and run through the above link.

## Video

Here is a short video describing our project and showing how you can work through the notebook.

https://youtu.be/DhkAs147cko 

## Data

The dataset for this data analysis project was aquired from Kaggle at this link: https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents?resource=download. It was compiled by Sobhan Moosavi.

We did not end up using the full dataset for our project, the features from the dataset that we used can be seen in this image.

![Picture1]([https://github.com/psu-edu/agile_stem_basic_game/assets/54818552/4730a87f-7b9f-46ae-bc83-d2e8c23b5ab7](https://github.com/Aidanjm13/USAccidentsDataAnalysis/blob/641bcc9bae67cfa24c0abbbf7d403dcca9418010/Images/DataSummary.png))

We also did some analysis of this data through summary statistics. In this graph you can see the distribution of the severity of accidents. The scale is in hundereds of thousands.

This chart shows some basic statistics of the data.

Finally we can look how the average data for each severity level here.

## Models

In order to better understand any relations between the data and to then be able to make predictions as to what conditions could cause more severe accidents, we built three models. 

The first model was a multiclass logistic regression model. The images below show the coefficient weights for the different features in the model which helps show which features contribute to the different severity of the accidents. From this we can see that features such as Distance, Temperature, Pressure, and the presence of objects such as stop lights or animal crossing all have major impacts on the severity of the accident.

The second model we made was a decision tree. Decision trees are highly explainable as we can see the the splits that it is making through graphs with the image below. This shows some of the initial major decisions made, with Accident length, traffic signal, and the distance of the accident being major factors.

We also made a neural network, and while the neural network was best at predicting the severity of the accident, they are also known as being black box models. 
For more information on these models and their effectiveness look at the Jupyter notebook linked above.

## Conclusions

This project explored factors that influence the severity of traffic accidents using real-world data and machine learning models. After cleaning and engineering features, we trained and evaluated logistic regressions, decision tree, and neural network models. Overall, accuracy was strong, at around 80-82%. However, predicting the rare high-severity accidents remained challenging due to class imbalance. The key features linked to accident severity included time of day, accident distance (miles), temperature(F), traffic signals, stop signs, crossings, and location. We can use thse insights to form infrastructure planning and road safety policies for local governments or larger councils. While our model performance on the most severe accidents was limited, the project lays a solid foundation for potential future improvements to better predict (and prevent) high-risk traffic scenarios.
