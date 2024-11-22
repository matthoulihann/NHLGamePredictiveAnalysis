NHL Matchup Predictor
Overview
The NHL Matchup Predictor is a Python-based application designed to predict the outcome of NHL games by analyzing team performance metrics. Leveraging machine learning with a Random Forest Classifier, the model predicts the win probabilities for two teams based on advanced hockey metrics.

Features
Win Probability Prediction: Predicts the likelihood of victory for two selected NHL teams.
Interactive Interface: Users can input team names and receive predictions dynamically.
Key Metrics: Analyzes hockey-specific statistics, including:
HDCF% (High Danger Chances For Percentage)
xGF% (Expected Goals For Percentage)
FF% (Fenwick For Percentage)
CF% (Corsi For Percentage)
SCF% (Scoring Chances For Percentage)
PDO (Shooting + Save Percentage)
Technical Details
Language: Python
Libraries:
pandas for data handling
sklearn for machine learning and evaluation
numpy for mathematical operations
Model Workflow

Data Preparation:
Extracts team performance statistics from a dataset.
Features are normalized to improve prediction accuracy.
Model Training:
Uses a Random Forest Classifier for robust predictions.
Splits data into training and testing sets for evaluation.
Prediction:
Accepts user input for two teams.
Outputs the predicted winner and win probabilities.

Follow the Prompts: Enter the names of two NHL teams to see their win probabilities and the predicted winner.

Example Usage
Welcome to the NHL Matchup Predictor!
Enter the name of the first team: Carolina Hurricanes
Enter the name of the second team: Chicago Blackhawks
The model predicts 'Carolina Hurricanes' to win.
Win Probabilities:
  Carolina Hurricanes: 87.32%
  Chicago Blackhawks: 12.68%
Do you want to predict another matchup? (yes/no): no
Thank you for using the NHL Matchup Predictor!

The model expects a dataset with the following columns:
Team: Name of the team
HDCF%, xGF%, FF%, CF%, SCF%, PDO: Performance metrics
W, L: Number of wins and losses (for labeling)
Ensure the dataset is saved as path_to_your_dataset.csv and properly preprocessed.

Evaluation
Accuracy: The model achieves high accuracy on test data (exact values depend on the dataset).
Evaluation Metrics:
Confusion Matrix
Precision, Recall, F1-Score
Future Enhancements
Live Data Integration: Connect the model to APIs for real-time game stats.
Player-Level Metrics: Incorporate individual player statistics for enhanced predictions.
GUI Application: Develop a user-friendly graphical interface.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Data is from https://www.naturalstattrick.com/teamtable.php

Contact
For inquiries, please contact Matthew Houlihan at mjhoulih@go.olemiss.edu.

