# SIFApplicationDataSet

Project Goal: Using given variables to predict whether a certain day was a holiday or not.

1. Correlation Heatmap and Bar Chart

A correlation heatmap was created from the given features.csv file. 
The variables in the file were taken and the correlation between each variable was mapped onto the heatmap.
Darker colors on the heatmap represents stronger negative correlations; on the other hand, lighter colors on the heatmap represents stronger positive correlations between variables.
The full heatmap can be seen on FULL_correlation_heatmap.png in the repository as well as the Data_Analysis.ipynb.

In addition, two bar charts were created to highlight the top 5 most positively correlated variables and the top 5 negatively correlated variables.
These charts are available on the head_correlation_bar_chart.png and tail_correlation_bar_chart.png files. The graphs can be more clearly viewed on the Jupyter Notebook file: Data_Analysis.ipynb.

The individual variables had low correlations with each other, so I decided to do a more complex analysis where more than one variable was used to predict an outcome variable. Intending to create a machine learning model, I decided to use the store number, department number, and weekly sales data from the test.csv file to predict whether a certain day was a holiday or not. The date was assigned to each row in the train.csv file; however, due to the format of the variable, the date was left out of the model. Furthermore, I chose to pick a simple model, a simple decision tree classifier.

2. Splitting training and testing data from the train.csv file. 

80% of the data was placed into the training set (output_train_x.csv and output_train_y.csv) and the remaining 20% of the data was placed into a testing set (output_test_x.csv and output_test_y.csv). The training and testing sets were created using the train_test_split function in the sklearn Python library. The code corressponding to this functionality is the third block of code in the Data_Analysis.ipynb file.

3. Preforming a cross validation on the decision tree classifier model from the sklearn library and testing hyperparameters (max leaf nodes and max depth of the decision tree).

Shown in the 




