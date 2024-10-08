# Customer Churn Prediction App

This repository contains a customer churn prediction app built with TensorFlow and Streamlit. The app predicts the likelihood of customer churn based on various user inputs such as geography, gender, age, balance, credit score, etc.

## Features

- **User Input via Streamlit:** The app collects user input for various features like Geography, Gender, Age, Balance, Credit Score, and more using interactive Streamlit widgets.
- **Model Predictions:** The app uses a pre-trained TensorFlow model to predict the probability of a customer churning.
- **Scalability:** Input features like gender and geography are preprocessed using label encoders and one-hot encoding, ensuring the model can handle categorical data effectively.
- **Prediction Display:** The churn probability is displayed as a result, along with a message indicating whether the customer is likely to churn.

## Files

- **`app.py`:** The main application code for running the Streamlit app. It includes loading the pre-trained model, user input handling, feature preprocessing, and displaying the prediction result.
- **`Churn_Modelling.csv`:** Dataset used for training the churn prediction model.
- **`experiments.ipynb`:** Jupyter notebook containing experiments related to model training, feature engineering, and evaluation.

## How to Run

1. Install the text file:
   ```bash
   pip install -r requirements.txt

2. Run the app
  ```bash
   streamlit run app.py
  ```

## Model
The model is a neural network built using TensorFlow and Keras, trained to predict customer churn. It uses features like:

- Geography (one-hot encoded)
- Gender (label encoded)
- Age
- Balance
- Credit Score
- Number of Products
- Has Credit Card (binary)
- Is Active Member (binary)
- Estimated Salary

## Usage

1. Open the web app. [Customer Churn Prediction App](https://ann-churn-classification-7x9snbrry3gappwr6arr26d.streamlit.app/)

## How it Works
1. The user inputs their data through the Streamlit interface.
2. The app preprocesses the inputs (encoding categorical data and scaling numerical data).
3. The pre-trained TensorFlow model predicts the probability of customer churn.
4. The app displays the churn probability and whether the customer is likely to churn or not.

## Files Description
- `app.py`: The script to run the Streamlit app for churn estimation. It handles user inputs, preprocessing, and model prediction​.
- `model.keras`: The pre-trained neural network model used for churn prediction.
- `onehotencoder_geography.pkl`: Pickle file containing the one-hot encoder for the Geography feature.
- `label_encoder_gender.pkl`: Pickle file containing the label encoder for the Gender feature.
- `scaler.pkl`: Pickle file containing the StandardScaler used for scaling numerical features.

The model was built using TensorFlow and the `model.keras` file stores the saved model, which is loaded during app runtime for predictions.

## Acknowledgments
This project was built using TensorFlow and Streamlit, with inspiration from various machine learning and data science resources.

## Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue if you find any bugs or want to improve the app.
