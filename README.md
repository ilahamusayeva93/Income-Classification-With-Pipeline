### Income Evaluation Project

#### Dataset Overview

The dataset used in this project, named 'income_evaluation.csv,' contains information about individuals, including features such as age, education, workclass, marital status, occupation, and sex. The target variable, 'income,' indicates whether an individual earns more than $50,000 annually.

#### Code Explanation

##### 1. Data Loading and Exploration

- Load the dataset using pandas (`pd.read_csv`).
- Initial exploration includes checking for null values, duplicates, and generating summary statistics.

##### 2. Data Preprocessing

- Remove duplicate rows (`df.drop_duplicates`).
- Apply label encoding to the 'income' column using `LabelEncoder`.
- Clean columns by stripping whitespaces and converting selected columns to the object type.

##### 3. Data Visualization

- Generate a pair plot and heatmap using seaborn (`sns.pairplot`, `sns.heatmap`) for visual exploration.

##### 4. Feature Engineering and Model Building

- Separate features into numeric and categorical types.
- Scale numeric features using `StandardScaler`.
- One-hot encode categorical features with `OneHotEncoder`.
- Implement a Gradient Boosting Classifier (`GradientBoostingClassifier`) using a pipeline (`Pipeline`) for preprocessing and model training.

##### 5. Model Evaluation

- Evaluate the model using accuracy and ROC-AUC scores.
- Utilize a precision-recall curve to find the best threshold for classification.
- Generate final predictions based on the chosen threshold.

##### 6. Model Serialization

- Save the trained model using `pickle.dump` for future use.
- Load the saved model back for making predictions (`pickle.load`).

#### How to Use

1. **Dependencies:**
   - Ensure required Python libraries are installed:
     ```
     pip install pandas numpy matplotlib seaborn scikit-learn
     ```

2. **Run the Code:**
   - Execute the code in a Jupyter Notebook or a Python script.
   - The code will load the dataset, preprocess the data, train the model, and provide evaluation metrics.

3. **Adjustments:**
   - Modify hyperparameters, add/remove features, or adjust the model architecture based on specific requirements


### Author

- Ilaha Musayeva

