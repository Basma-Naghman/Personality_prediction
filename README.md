
🧠 Personality Prediction using Decision Tree Classifier
This project predicts whether a person is an Introvert or Extrovert using a dataset of social behavior metrics. It utilizes a DecisionTreeClassifier from scikit-learn, with preprocessing handled through a ColumnTransformer and a Pipeline.

📌 Problem Statement
Given features like:

Time spent alone

Stage fear

Social event attendance

Feeling drained after socializing

Friends circle size

Frequency of social media posts

...we aim to predict a person’s personality type: Introvert or Extrovert.

🔧 Tech Stack
Python 🐍

NumPy

Pandas

scikit-learn

Matplotlib (for visualization)

📂 Dataset Features
Feature	Type	Description
Time_spent_Alone	Numeric	Hours spent alone
Stage_fear	Categorical	Yes/No for fear of public speaking
Social_event_attendance	Numeric	Number of events attended
Going_outside	Numeric	Frequency of going outside
Drained_after_socializing	Categorical	Yes/No for feeling drained after socializing
Friends_circle_size	Numeric	Number of close friends
Post_frequency	Numeric	Social media activity level
Personality (Target)	Categorical	Introvert / Extrovert

🚀 How It Works
Preprocessing:

OneHotEncoder is applied to categorical features.

All others are passed through unchanged using remainder='passthrough'.

Model Training:

A DecisionTreeClassifier is trained using a pipeline.

The target (Personality) is label-encoded.

Evaluation:

Accuracy score

Confusion matrix for visualization
