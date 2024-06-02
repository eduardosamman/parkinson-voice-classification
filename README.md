# parkinson-voice-classification

This script is designed to detect Parkinson's disease using machine learning techniques. It uses a variety of Python libraries to process and analyze data, train a model, and evaluate its performance.

## Libraries Used  

numpy: Used for numerical operations.  
pandas: Used for data manipulation and analysis.  
matplotlib.pyplot: Used for creating static, animated, and interactive visualizations in Python.  
seaborn: Used for statistical data visualization based on matplotlib.  
sklearn.model_selection: Used for splitting the dataset into training and testing sets, K-Fold cross-validation, and scoring the cross-validation.  
sklearn.preprocessing: Used for preprocessing the dataset, specifically for feature scaling.  
sklearn.metrics: Used for evaluating the model, specifically for creating a confusion matrix.  
sklearn.decomposition: Used for applying Principal Component Analysis (PCA), a dimensionality reduction technique.  
catboost: Used for implementing the CatBoost Classifier, a machine learning algorithm that uses gradient boosting on decision trees.  
imblearn.over_sampling: Used for handling imbalanced classes in the dataset.  

## How to Run  
To run this script, you need to have Python installed on your machine along with the above-mentioned libraries. You can then run the script using a Python interpreter or an integrated development environment (IDE) like Jupyter Notebook or Visual Studio Code.

Please note that this script assumes you have a specific dataset in a specific format. Make sure to adjust the data loading and preprocessing steps according to your dataset.
<p>The following script provides a comprehensive approach to classify Parkinson's disease patients from healthy individuals using machine learning techniques. The workflow involves several key steps:</p>
<ul>
    <li><b>Data Loading</b>: The script starts by loading the dataset containing features that are used to distinguish between Parkinson's patients and healthy controls.</li>
    <li><b>Preprocessing</b>: Preprocessing steps are crucial for preparing the data for analysis. This includes handling missing values, normalizing the data, and encoding categorical variables if necessary.</li>
    <li><b>Data Augmentation with RandomOverSampler</b>: To address the issue of class imbalance in the dataset, the script utilizes the RandomOverSampler technique. This method helps in balancing the dataset by oversampling the minority class, ensuring that the classifier does not become biased towards the majority class.</li>
    <li><b>Principal Component Analysis (PCA)</b>: PCA is applied to reduce the dimensionality of the dataset while retaining most of the variance. This step helps in improving the efficiency of the model and can also aid in visualizing the data more effectively.</li>
    <li><b>Classification using CatBoost</b>: Finally, the script employs the CatBoost algorithm, a state-of-the-art gradient boosting method that handles categorical features efficiently and is robust to overfitting. CatBoost is used to build a classifier that can accurately distinguish between Parkinson's disease patients and healthy individuals.</li>
