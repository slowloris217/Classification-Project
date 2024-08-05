# Classification-Project

This project aims to predict customer churn for a fictional telecommunications company using a [dataset](churn.xlsx)  containing various customer attributes and their churn status. 
More information can be found here.

The goal is to create a model to predict whether or not a customer will churn based on their profile and behavior.
To achieve this, we employed three different machine learning models : Random Forest Classifier, Logistic Regression, and Support Vector Classifier (SVC). 

We evaluated the models using metrics such as accuracy, precision, recall, F1-score, and the area under the precision-recall curve (AUC-PR). Cross-validation was used to ensure the models' performance was consistent across different data splits as well as hypertuning parameters to obtain the best results.

Random Forest outperformed the other models in most metrics, offering the highest accuracy, making it the best choice for our churn prediction task.

Using the random forest as our final model, we wanted to see what the model would predict given a new set of inputs. Taking a row from the dataset, values such as Contract, Churn Score, Gender, Total Charges and Tenure Months were modified and then given to the model. Originally, the data row had a Churn value of 1, but the model had deemed the new modified row as not churned despite the increase in churn score. Implying the effects of the other modified features were much more significant in this case.

In conclusion, it demonstrates the importance of looking at multiple variables for our classifications models and how observing one variable isn’t always enough to make predictions.

### Notebook content
1. Import Necessary Libraries, Reading, Exploring and Preparing Data
2. Create Random Forest Classifier model
3. Create Logistic Regression model
4. Create Support Vector Classifier (SVC) model
5. Make prediction
    - We chose one model and tested it on a sample customer to predict the likelihood of churn.




### Files Included
- .ipynb Notebook
- CSV file
