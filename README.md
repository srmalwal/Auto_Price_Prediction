# Auto_Price_Prediction

A machine learning web application that predicts automobile prices from vehicle attributes. This repository contains the auto dataset, a Jupyter Notebook for data preparation and model development, a saved Random Forest model, and a Streamlit application for making predictions.

## Features

- Predicts an estimated automobile price from user-provided vehicle details.
- Provides an interactive Streamlit interface.
- Loads a saved machine learning model and the feature information needed for prediction.
- Includes a Jupyter Notebook for data analysis and model experimentation.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Streamlit
- Jupyter Notebook
- Pickle for saved model artifacts

## Dataset

The project uses `autos_dataset.csv`.

Check the dataset headers and notebook for the exact features and target column used in this implementation. The application expects vehicle-related input fields that match the trained model's features.

## Machine Learning Model

The saved model is:

```text
random_forest_model.pkl
```

The application uses this trained model to generate predictions. The notebook named `Linear regression_Auto Data Set.ipynb` documents the model-development workflow and may include linear regression experiments as well as data preprocessing and evaluation.

Model performance metrics should be taken from the notebook's actual evaluation output; this README does not assume an accuracy or error score.

## Repository Structure

```text
Auto_Price_Prediction/
├── app.py
├── autos_dataset.csv
├── Linear regression_Auto Data Set.ipynb
├── random_forest_model.pkl
├── features.pkl
└── README.md
```

The uploaded files may contain suffixes such as `(2)` or timestamps in their local names. Use the clean names shown above in the GitHub repository, and update references in the code if you choose different filenames.

## Installation

Install the libraries required to run the application:

```bash
pip install streamlit pandas numpy scikit-learn
```

If you plan to run the notebook, also install Jupyter:

```bash
pip install notebook
```

## Run the Application

Place `app.py`, `random_forest_model.pkl`, and `features.pkl` in the same project directory, then run:

```bash
streamlit run app.py
```

Open the local URL printed in the terminal by Streamlit.

## How to Use

1. Start the Streamlit application.
2. Enter the vehicle details requested by the interface.
3. Submit the form to generate a price prediction.
4. Review the estimated price displayed by the application.

The exact input fields and prediction formatting are defined in `app.py`.

## Project Files

| File | Purpose |
|---|---|
| `app.py` | Streamlit user interface and prediction logic |
| `autos_dataset.csv` | Automobile dataset |
| `Linear regression_Auto Data Set.ipynb` | Data exploration, preprocessing, and model development |
| `random_forest_model.pkl` | Saved Random Forest model |
| `features.pkl` | Saved feature information used by the application |
| `README.md` | Project documentation |

## Limitations

- Predictions depend on the coverage and quality of the dataset.
- Vehicle prices can vary with location, condition, mileage, and market changes that may not all be represented in the input data.
- The output is an estimate, not a guaranteed selling price.
- The saved model and feature file must remain compatible with the preprocessing and input order expected by the app.
- Only load Pickle files from trusted sources.

## Future Improvements

- Display validated model evaluation metrics in the application.
- Add input validation and clearer error messages.
- Compare multiple regression models on the same test split.
- Tune model hyperparameters using cross-validation.
- Add visualizations for dataset trends and prediction errors.
- Deploy the application online.

## Conclusion

`Auto_Price_Prediction` demonstrates a machine learning workflow for automobile price estimation, from dataset exploration and model development to saved model artifacts and an interactive Streamlit application.
