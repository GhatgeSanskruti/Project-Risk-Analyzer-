# Project Outcome Prediction Model

This project uses a Decision Tree classifier to predict whether a project will be a "Success" or "Failure" based on key project management inputs.

The notebook loads a project dataset, preprocesses the categorical features using `LabelEncoder`, and then trains three separate models to demonstrate the bias-variance tradeoff:
1.  **Overfit Model:** A Decision Tree with no constraints.
2.  **Underfit Model:** A Decision Tree with `max_depth=1`.
3.  **Good Fit Model:** A Decision Tree with `max_depth=4`.

The notebook also includes an interactive prompt that allows a user to input their own project details and receive a live prediction.

## Key Features

* **Model Training:** Demonstrates the difference between an overfit, underfit, and balanced model.
* **Performance Evaluation:** Uses Accuracy, Classification Reports, and Confusion Matrices to evaluate the "Good Fit" model.
* **Feature Importance:** Analyzes and plots which project factors are the most important for predicting the outcome.
* **Interactive Prediction:** A user-friendly prompt (Cell 10) allows you to enter your own project's factors and get a real-time prediction.

## Dataset

* **File:** `project_dataset_100.csv` (Not included in this repo)
* **Features (Inputs):**
    * `ClarityOfObjectives`
    * `PlanningDetail`
    * `ResourceAvailability`
    * `DeadlineRealism`
    * `CommunicationFrequency`
    * `StakeholderEngagement`
    * `RiskManagementPlan`
    * `ScopeControlProcess`
* **Target (Output):**
    * `PredictedOutcome` (Success / Failure)

## How to Use

1.  Clone this repository.
2.  Make sure you have the required libraries installed (see `requirements.txt`).
3.  Place your `project_dataset_100.csv` file in the same directory.
4.  Run the `project_predictor.ipynb` notebook (it's recommended to rename `FINAL FINAL!!!.ipynb` to this).
5.  Follow the interactive prompts at the end of the notebook to get a prediction.

## Dependencies

This project requires the following Python libraries:
* pandas
* numpy
* scikit-learn
* matplotlib
