# Projects Show Reel
Examples of projects done during the Data Science Course at Practicum100 by Yandex.

### Telecom:
In this project, we studied data provided by a telecom company to train a model that would predict the churn of clients. The company would like to know in advance which customer is more likely to churn so they could offer benefits to encourage the customer to stay active, a binary classification problem.

#### Challenges
There were quite a few challenges in this project regarding data preparation and pre-processing.

Not all of the provided data sets were of the same length, as a result, the merge of these tables produced NaN values in various services in over 20% of the data. That is significant, moreover that it is not a large data set.
The data represented a class imbalance between customers that already left (the minority) to data on clients that are still active (the majority)
Training and optimizing different models to reach the required threshold, building a pipeline, using GridSearchCV to identify the best hyperparameters combination and an evaluation function for each model.
