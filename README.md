Project Overview: 

This project focuses on building a machine learning classification model to predict the acceptability of cars based on their characteristics.

The goal is to determine whether a car is:
- Unacceptable
- Acceptable
- Good
- Very Good

The project uses a Decision Tree classifier to learn patterns from the dataset and predict the class of new observations.

This project demonstrates key data science workflow steps, including:
- Data exploration
- Data preprocessing
- Encoding categorical variables
- Model training
- Model evaluation

Dataset

The dataset comes from the UCI Machine Learning Repository. 

Dataset: Car Evaluation Dataset
url : http://archive.ics.uci.edu/ml/datasets/Car+Evaluation

It contains categorical variables describing cars and a target variable indicating their acceptability.
Features: 
| Feature  | Description                  |
| -------- | ---------------------------- |
| buying   | Buying price                 |
| maint    | Maintenance price            |
| doors    | Number of doors              |
| persons  | Capacity in terms of persons |
| lug_boot | Luggage boot size            |
| safety   | Safety level                 |

Target variable: 
| Class | Meaning      |
| ----- | ------------ |
| unacc | Unacceptable |
| acc   | Acceptable   |
| good  | Good         |
| vgood | Very Good    |

Technologies Used
- Python
- Pandas – Data manipulation
- NumPy – Numerical operations
- Matplotlib / Seaborn – Data visualization
- Scikit-learn – Machine learning
- Category Encoders – Categorical encoding

Project Workflow : 

1️⃣ Data Loading
The dataset is imported and inspected to understand:
- Data structure
- Feature types
- Distribution of categories

2️⃣ Data Preprocessing
Key preprocessing steps include:
- Column renaming
- Checking for missing values
- Feature/target separation
- Train/Test split

Dataset split:
- Training set: 67%
- Test set: 33%

3️⃣ Encoding Categorical Variables
Since all features are categorical, they must be converted into numerical format before training the model.

This project uses an Ordinal Encoder to transform categories into numerical values.

Machine Learning Model
A Decision Tree Classifier is used to perform the classification.

Two models are trained and compared.
Model 1 — Decision Tree (Gini Index)
Parameters:
criterion = "gini"
max_depth = 3

The Gini impurity measures the probability of incorrectly classifying a randomly chosen element.

Model 2 — Decision Tree (Entropy)
Parameters:
criterion = "entropy"
max_depth = 3

Entropy measures the information gain at each split in the tree.

Model Evaluation

The models are evaluated using:
- Accuracy Score
- Train vs Test Accuracy
- Confusion Matrix

The confusion matrix helps identify:
- Correct predictions
- Misclassifications

Visualizations
The project includes visualizations to better understand the model performance:
- Feature distributions
- Confusion matrix heatmap
- Model performance comparison

Project Structure

car-evaluation-ml

│

├── evaluation_voiture.ipynb   # Main notebook

├── car.data                   # Dataset

├── README.md                  # Project documentation

Learning Objectives
This project demonstrates practical skills in:
- Data preprocessing
- Handling categorical variables
- Supervised machine learning
- Model evaluation
- Data visualization

These skills are essential for Data Analysts and Data Scientists.

Possible Improvements
Future improvements could include:
- Testing additional models:
  - Random Forest
  - Gradient Boosting
  - Logistic Regression


