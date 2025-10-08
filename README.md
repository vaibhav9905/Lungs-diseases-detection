🫁 Lung Cancer Detection Model 🔬
🌟 Project Overview
This project implements a machine learning solution to predict the risk of Lung Cancer based on an individual's symptoms and lifestyle factors. By analyzing survey data, we built and evaluated a classification model to provide insights into potential health risks.

This notebook documents the entire process, from Data Preprocessing and Exploratory Data Analysis (EDA) to Model Training and Evaluation.

📊 Dataset & Features
The model uses a survey dataset containing various features, which are mostly binary (1 for 'Yes', 0 or 2 for 'No'/'Other' depending on the feature) or categorical, and one numerical feature (Age).

Key Features Used:
GENDER 🧑 / 👩

AGE 🎂

SMOKING 🚬

YELLOW FINGERS 🖐️

ANXIETY 😨

PEER PRESSURE 🤝

CHRONIC DISEASE 🤒

FATIGUE 😴

ALLERGY 🤧

WHEEZING 💨

ALCOHOL CONSUMING 🥃

COUGHING 😷

SHORTNESS OF BREATH 🥵

SWALLOWING DIFFICULTY 嚥

CHEST PAIN 💔

Target Variable: LUNG CANCER (1: Yes, 0: No)

🛠️ Methodology & Techniques
1. Data Preparation
Encoding: Categorical features like GENDER and the target variable LUNG CANCER were converted to numerical representations using Label Encoding.

Splitting: The data was split into training and testing sets (80% train, 20% test) to ensure robust model evaluation.

Scaling: Numerical features (like AGE and the transformed binary/categorical columns) were normalized using StandardScaler to prevent feature dominance and improve model performance.

2. Model Training
Logistic Regression: A baseline classification model was trained and evaluated first.

Support Vector Classifier (SVC): An SVC model was trained and provided the final, highly accurate predictions.

3. Evaluation
Confusion Matrix: Visualized to understand the breakdown of correct and incorrect predictions.

Classification Report: Used to calculate key performance metrics like Precision, Recall, and F1-score.

📈 Results & Performance
The Support Vector Classifier (SVC) model achieved outstanding performance on the test data:

Metric

Score

Insight

Test Accuracy

96.77%

The model correctly predicted the outcome nearly 97% of the time.

Train Score

85.02%

Good generalization capability.

Recall (Class 1 - Cancer)

1.00

Crucially, the model successfully identified 100% of the actual positive lung cancer cases in the test set (no False Negatives for this class).

F1-Score (Class 1 - Cancer)

0.98

A high score indicating strong balance between precision and recall.

Visualizations Included:
Distribution of the Target Variable (LUNG_CANCER).

Distribution of AGE.

Pairwise relationships between key features (AGE, SMOKING, YELLOW_FINGERS, ANXIETY).

Correlation Heatmap of all numerical features.

🚀 How to Run the Notebook
This project was developed using a Google Colab environment.

Clone the Repository (if applicable) or download the notebook file.

Upload the notebook to Google Colab.

Ensure the dataset (survey lung cancer.csv) is accessible in the Colab environment (e.g., uploaded to /content/).

Run all cells sequentially.

Prerequisites
Python 3.x

pandas

numpy

matplotlib

seaborn

scikit-learn (sklearn)
