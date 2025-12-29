I am a data scientist and I need to make a prediction about survival on Titanic dataset. The metric to predict is "Survived" in the dataset and you must be predict whether a passenger survived or not. In terms of models, you must use Logistic Regression, Random Forest and XGBoost. In terms of metrics, you must use AUC and ROC curves. 

Take as much time as you need to complete the task: I value quality over speed, i expect detailed EDA with charts on all metrics and clear next steps on how to improve the models. The focus is the Jupyter notebook output and the Python code. Do not build any fancy UI with charts.

The document is intended for a non data scientists audience so please explain in plain english the output. 

Features
1. Include a feature to import csv and 
2. a feature to export a Jupyter notebook as output and 
3. display all Python code as Jupyter notebook output as well. 

The csv will be in the same folder than the Jupyter notebook, keep it in mind when writing the code to import the file.

Please take as much time as you need to complete the following steps for the model
1. Load all libraries
2. Load the dataset
3. Dataset exploration
a. Investigate the relationship between features and target variable for each feature with charts
b. Look for Correlation between categorical and numerical values with charts for each feature
c. Have a look at Missing values and detect whether it is missing at random or not with charts for each feature
d. Categorical value occurrence analysis with charts for each feature
e. Add a correlation matrix to the field we want to predict.
f. For highly correlated features to the field to predict, explore ways to improve the AUC
g. Look for distribution for each numerical feature and report outliers
h. Write up all your findings
4. Data engineering
a. Turn your findings from EDA into feature engineering and transform features to protect from outliers
b. Do not run any imputation on data at this stage: it will cause data leakage and compromise the model
5. Preprocessing
a. Split the dataset into training dataset,test dataset and validation dataset with 60/20/20 ratio. Do not override this instruction no matter what. It takes two splits in Python to do that.
b.Create a pipeline to apply transformation and use imputation on features where it makes sensincluding advanced methods like MICE or synthetic data but don't make the mistake to create a data leakage:  apply the imputation on the training dataset in isolation and not the test/validation dataset.
c. Use SMOTE on class imbalance
d. Apply pre-processing on data
6. Fine tune models
a. Run hyperparameter tuning on Logistic Regression, Random Forest and XGBoost
b. Work on dynamic Ensemble based on best models
7. Model Evaluation on AUC and ROC curves for the 3 models and the Ensemble
8. Run SHAP interpretability  on the 3 models and the Ensemble with findings. Make sure to do it on the 3 models and the Ensemble and be careful not to mess up with the scaled version.
9. Look at false positive and provide next steps with detailed instructions to improve models


On all model steps, include AUC.

Make one final check to make sure 
1. the Jupyter export is working and
2. the Python code runs without error

And again, be very careful on the Jupyter export so take extra time on this task