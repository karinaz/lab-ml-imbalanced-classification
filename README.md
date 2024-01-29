<p style="font-size: 16px;">For this lab we will build a model on customer churn binary classification problem. You will be using&nbsp;<a href="https://drive.google.com/file/d/1C58ntdJEsDIPt0a0FKUWeqTQ-2A8KnHw/view?usp=share_link" target="[object Object]">DATA_Customer-Churn&nbsp;</a>file that you can find in this&nbsp;<a href="https://drive.google.com/file/d/1C58ntdJEsDIPt0a0FKUWeqTQ-2A8KnHw/view?usp=share_link" target="[object Object]">LINK</a>.</p>
<p style="font-size: 16px;"><strong>Scenario</strong></p>
<p style="font-size: 16px;">You are working as an analyst with this internet service provider. You are provided with this historical data about your company's customers and their churn trends. Your task is to build a machine learning model that will help the company identify customers that are more likely to default/churn and thus prevent losses from such customers.</p>
<p style="font-size: 16px;"><strong>Instructions</strong></p>
<p style="font-size: 16px;">In this lab, we will first take a look at the degree of imbalance in the data and correct it using the techniques we learned on the class. Here is the list of steps to be followed (building a simple model without balancing the data):</p>
<p style="font-size: 16px;"><strong>Round 1</strong></p>
<ul>
<li>&nbsp;Import the required libraries and modules that you would need.</li>
<li>Read that data into Python and call the dataframe churnData.</li>
<li>Check the datatypes of all the columns in the data.You would see that the column TotalCharges is object type. Convert this column into numeric type using pd.to_numeric function.</li>
<li>Check for null values in the dataframe. Replace the null values.</li>
<li>Use the following features: tenure, SeniorCitizen, MonthlyCharges and TotalCharges:</li>
<ul>
<li>Split the data into a training set and a test set.</li>
<li>Scale the features either by using MinMaxScaler or a standard scaler.</li>
</ul>
<li>(Optional) Encode the categorical variables so you can use them for modeling later.</li>
</ul>
<p style="font-size: 16px;"><strong>Round 2</strong></p>
<ul>
<li>(Optional) Fit a logistic Regression model on the training data.</li>
<li>Fit a Knn Classifier (NOT KnnRegressor please!)model on the training data.</li>
<li>Fit a Decision Tree Classifier on the training data.</li>
<li>Compare the accuracy, precision, recall for&nbsp;the previous models on both the train and test sets.</li>
</ul>
<p style="font-size: 16px;"><strong>Round 3</strong></p>
<ul>
<li>apply K-fold cross validation on your models&nbsp;built before,&nbsp;&nbsp;and check the model score. Note: So far we have not balanced the data.</li>
</ul>
<p style="font-size: 16px;"><strong>Round 4</strong></p>
<ul>
<li>fit a Random forest Classifier on the data and compare the accuracy.</li>
<li>tune the hyper parameters with Gridsearch and check the results. retrain the final mode with the best parameters found.</li>
</ul>
<p style="font-size: 16px;"><strong>Managing imbalance in the dataset</strong></p>
<ul>
<li>Check for the imbalance.</li>
<li>Use the resampling strategies used in class for upsampling and downsampling to create a balance between the two classes.</li>
<li>Each time fit the model and&nbsp;check&nbsp;the accuracy of the model.</li>
</ul>
