# Airbnb_Price_Prediction
Statistical Learning Project KNN

9/22/2021
We are using the California Housing price dataset. The dataset is derived from the 1990 census and shows the median house price of California districts. Further information on the dataset can be find in this link:https://www.kaggle.com/camnugent/california-housing-prices.



In using this dataset, we aim to predict the median price of a given house using its number of accommodates, bathrooms, bedrooms, and beds as the predictors.

<img width="776" alt="Screen Shot 2022-01-15 at 4 02 09 PM" src="https://user-images.githubusercontent.com/93837295/149637604-3ca709b3-20d8-45df-b78f-6d950b15ce31.png">

To determine the most optimal k value for our model, we used leave-one-out cross-validation to determine the optimal k value with the least error. We first calculated the difference between our predicted house price and its actual value for each row. We then calculated the average of its squared error for a given k value. We repeated this process k value between 1 and 50. Then by plotting the average error against each K value, we can visualize the change of our model’s accuracy as we increase the k value. Specifically, we find that the mean squared error decreases rapidly after the first few k values. This is because the average of 3 or more values will be a more accurate prediction than just finding the single nearest neighbor. However, as the number of k nearest neighbor further increases, we find that its effect of improving the model’s accuracy diminishes and eventually mean squared error increases. In the end, for the 150 total k values investigated, we spotted the k value that gives us the minimal mean squared error is 43.

<img width="808" alt="Screen Shot 2022-01-15 at 4 02 52 PM" src="https://user-images.githubusercontent.com/93837295/149637622-e6619bd2-1d28-4cd2-a02d-47a38a39ae65.png">

<img width="803" alt="Screen Shot 2022-01-15 at 4 03 06 PM" src="https://user-images.githubusercontent.com/93837295/149637628-732bc04e-65e8-4db5-937a-44dbf5ecf767.png">
