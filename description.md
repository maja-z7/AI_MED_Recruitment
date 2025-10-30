## Models selection
In my experiments I've decided to test three different models: Linear Regression, K-Nearest Neighbors and Random Forest. 

## Program structure 
First, I load the data from csv file and split it for training and testing (80% and 20%).

Then, for every model, I go through the same steps
1. Hyperparameters tunning
2. Model trainng
3. Solution evaluation

## Results discussion
We can see that Logistic Regression model achieved the highest result - 75%. The results are lower than the ones we got in cross-validation. That is because before we worked only with the training dataset, so the performance was lower when we evaluated the model on unseen data. We can see how well the models performed on the graphs (ROC curve). Each point on the curve corresponds to a specific decision threshold. A perfect model would have a curve that goes to the top-left corner, while a random guess would result in a straight diagonal line from the bottom-left to the top-right. Another reason for lower results might be a pretty small size of the dataset. That is why we achieved exactly the same result in KNN and Random Forest (62.5%). The dataset was split into training set (80%) and testing set (20%) and since the dataset is small we got only a few examples (8 to be precise) for testing, therefore the results are not very diverse.