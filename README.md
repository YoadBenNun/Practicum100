# Projects Show Reel
Examples of projects done during the Data Science Course at Practicum100 by Yandex.

## 💡 Telecom Churn Project:
In this project, we studied data provided by a telecom company to train a model that would predict the churn of clients. The company would like to know in advance which customer is more likely to churn so they could offer benefits to encourage the customer to stay active, a binary classification problem.

#### ⛳️ Challenges:
There were quite a few challenges in this project regarding data preparation and pre-processing.

Not all of the provided data sets were of the same length, as a result, the merge of these tables produced NaN values in various services in over 20% of the data. That is significant, moreover that it is not a large data set.
The data represented a class imbalance between customers that already left (the minority) to data on clients that are still active (the majority)
Training and optimizing different models to reach the required threshold, building a pipeline, using GridSearchCV to identify the best hyperparameters combination and an evaluation function for each model.


## 💡 Machine learning, efficiency and gold recovery from ores Project:
In this project, we studied data provided by a metal mining company to train a model that would predict the most efficient process to extract gold out of ores.
Based on data collected by IoT sensors along the production line we can estimate the concentrations and amounts of different substances and techniques needed to extract the most gold out of the ores.

#### ⛳️ Challenges:
There were quite a few challenges in this project regarding data preparation and pre-processing.

- The data provided had a high portion of missing values in different parts of the datasets.
- The data provided had a high dimensionality due to a complex process of production.
- The missing values in our data were quite random, each production is different, with different input, and different processes of extraction. That made filling these values quite a challenge.
- Due to a complex production process, our metric of evaluation had to be custom-made to evaluate the model’s performance.
