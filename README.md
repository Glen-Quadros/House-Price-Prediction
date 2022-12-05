# House-Price-Prediction-using-Advanced-Regression-Techniques

This project is from Getting Started competitions from kaggle. The train and test dataset was downloaded from kaggle. 

In this project, I read the train .csv fil using pandas python library. I then proceed to visualize the data with help of the Seaborn Python library. By visualizing the data, I remove certain outliers. 

I then proceed to check if the dataset has any sort of missing data. With the help of data_description.txt file, I fill in the missing data. 

After that, I read in the test.csv file and procedd to drop unnecessary columns. Since the shape of train dataframe does not match the shape of test dataframe, I create a new variable which take the train dataframe columns as a list and then align it with test dataframe and fill the remaining values with 0.

I then use the Gradient Boosting MAchine Learning model and then with the help of GridSearchCV, I find the best parameters for the model. I use negative root mean squadred error as the scoring metric. After being satisfied with the machine learning model, I then proceed to make a final model using the parameters I got from the GridSearchCV. I then proceed to make predictions using the final model and then store it in a Pandas DataFrame. I finally save the predictions to a submission_gb.csv file
