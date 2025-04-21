# README for AI_Home.ipynb

## Overview
This Jupyter Notebook (`AI_Home.ipynb`) demonstrates a simple linear regression model for predicting house prices based on features such as square footage, number of bedrooms, bathrooms, and offers. The dataset used is `house-prices.csv`.

## Dependencies
To run this notebook, ensure you have the following Python libraries installed:
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`

You can install these dependencies using pip:
```bash
pip install numpy pandas scikit-learn matplotlib
```

## Dataset
The dataset (`house-prices.csv`) contains the following columns:
- `Home`: Identifier for the house.
- `Price`: Target variable representing the house price.
- `SqFt`: Square footage of the house.
- `Bedrooms`: Number of bedrooms.
- `Bathrooms`: Number of bathrooms.
- `Offers`: Number of offers received.
- `Brick`: Whether the house is made of brick (not used in the model).
- `Neighborhood`: Neighborhood of the house (not used in the model).

## Code Workflow
1. **Data Loading and Exploration**: The dataset is loaded and basic statistics are displayed using `df.describe()`.
2. **Feature Selection**: The features `Home`, `SqFt`, `Bedrooms`, `Bathrooms`, and `Offers` are selected for the model, while `Price` is the target variable.
3. **Train-Test Split**: The data is split into training and testing sets with a 90% test size.
4. **Model Training**: A linear regression model is trained on the training data.
5. **Prediction**: The model is used to predict house prices for the test set.
6. **User Input**: The model can also predict the price for user-provided input features.

## Usage
1. Run the notebook cells in sequence to load the data, train the model, and make predictions.
2. To predict the price for a custom house, provide the following features when prompted:
   - Home identifier
   - Square footage
   - Number of bedrooms
   - Number of bathrooms
   - Number of offers

## Example Output
The notebook outputs the predicted prices for the test set and can display a prediction for user input. For example:
```python
[142383.46559984]
```

## Notes
- The model uses a simple linear regression approach and may not capture complex relationships in the data.
- The test size is set to 90%, which is unusually high; consider adjusting this for better model evaluation.
