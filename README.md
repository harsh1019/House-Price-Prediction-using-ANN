### Table of Contents

1. Introduction
2. Data Preprocessing
3. Neural Network Architecture
4. Model Training
5. Model Evaluation
6. Web Application using Flask
7. Documentation for Flask App

### Introduction
The House Price Prediction System is designed to forecast house prices by analyzing various features such as location, room details, and amenities. This system employs a neural network model created with the Keras framework. To enhance usability, a Flask web application has been developed, allowing users to input data and receive price predictions seamlessly.

### Data Preprocessing
#### Data Scaling:
Features are standardized using the Min-Max Scaler from scikit-learn to ensure uniform input for the neural network.
#### Data Splitting:
The dataset is divided into training and testing sets to accurately assess the model's performance.

### Neural Network Architecture
The neural network consists of an input layer, two hidden layers with dropout for regularization, and an output layer designed for regression tasks.

- **Input Layer:** 1000 neurons, ReLU activation
- **Dropout Layer:** 20% dropout rate
- **Hidden Layer 1:** 500 neurons, ReLU activation
- **Dropout Layer:** 20% dropout rate
- **Hidden Layer 2:** 250 neurons, ReLU activation
- **Output Layer:** 1 neuron, linear activation for regression

### Model Training
The model is compiled using the RMSprop optimizer and the Mean Squared Error (MSE) loss function. Early stopping is utilized with a patience of 50 epochs to avoid overfitting. The model is trained over 10 epochs with a batch size of 50.

### Model Evaluation
The model's performance is evaluated using several metrics, including:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Mean Squared Log Error (MSLE)
- R-squared score

These metrics are applied to the testing dataset to ensure accurate evaluation.

### Web Application using Flask
A user-friendly Flask web application has been developed to predict house prices. This application loads the pre-trained neural network model and scaler, allowing users to input features like longitude, latitude, and house age, and receive predicted house prices.

### Documentation for Flask App
Comprehensive documentation has been provided to guide users through the features and functionalities of the Flask web application, ensuring ease of use and understanding.
