<h1>Credit Card Fraud Detection Python</h1>

<h2>Project Overview</h2>
This project develops a fraud detection model that can predict fraudulent credit card transactions based on the credit card dataset provided. The dataset contains 31 columns, which include transaction time, transaction amount, and 28 anonymized features (V1-V28). The dataset has 284,807 rows and two classes, 0 and 1, where 0 means that the transaction is not fraudulent and 1 means that the transaction is fraudulent.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b>
- <b>JupiterLabs</b>

<h2>Environments Used </h2>

- <b>Anaconda</b> 

<h2>Program walk-through:</h2>

<p align="center">
  <h3>Data Exploration:</h3>
We used Pandas to read the CSV file and print the first few rows of the data. We also checked the distribution of the target variable using value_counts() method and found that the dataset is highly imbalanced with 284,315 transactions labeled as non-fraudulent and only 492 transactions labeled as fraudulent.: <br/>
<img src="https://imgur.com/Oe8FPMM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Model Development:</h3>
We used Scikit-Learn's DecisionTreeClassifier to build a machine learning model for fraud detection. First, we split the data into training and testing sets with a test size of 20% and a random state of 42. Next, we instantiated a DecisionTreeClassifier model with a random state of 42 and trained it on the training data. We then made predictions on the test data and calculated the accuracy of the model using the accuracy_score() method. We achieved an accuracy of 99.91%, which is high, but not a reliable measure of the model's performance because of the imbalanced dataset.
: <br/>
<img src="https://imgur.com/Os2uyXw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Model Evaluation:</h3>
We evaluated the performance of the model using a confusion matrix, which is a table that shows the true positive, true negative, false positive, and false negative values of the model's predictions. We used Scikit-Learn's confusion_matrix() method to calculate the confusion matrix, which showed that the model correctly classified 56,830 non-fraudulent transactions and 78 fraudulent transactions, while misclassifying 20 non-fraudulent transactions and 34 fraudulent transactions. This indicates that the model performs well on non-fraudulent transactions but has a higher false negative rate for fraudulent transactions.
: <br/>
<img src="https://imgur.com/AkxieeF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br /> <h3>Data Visualization:</h3>
We created two visualizations to explore the data. The first visualization is a scatter plot of the transaction amount against the transaction time, which shows that there is no significant relationship between the two variables. The second visualization is a bar chart of the number of non-fraudulent and fraudulent transactions in the dataset, which confirms that the dataset is highly imbalanced. The heatmap makes it easier to visualize this information by color-coding the cells according to the frequency of predictions in each cell. Therefore, the accuracy metric should be used with caution, as it can be misleading in imbalanced datasets. 
: <br/>
<img src="https://imgur.com/pdzREJt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://imgur.com/3VyQGTn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://imgur.com/38tYpnK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
