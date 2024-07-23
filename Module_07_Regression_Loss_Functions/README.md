# Regression Loss Functions

## Topics covered in today's module
* Mean Squared Error
* Mean Absolute Error
* Mean Squared Logarithm Error

## Main takeaways from doing today's assignment

## Understanding Loss Functions
Loss functions define the discrepancy between predicted and actual values, guiding the optimization process during model training. They are pivotal in quantifying how well a model's predictions align with ground truth data.

## Types of Regression Loss Functions
- Mean Squared Error (MSE)
MSE measures the average squared difference between predicted and actual values. It emphasizes larger errors due to squaring, making it suitable for tasks where precise prediction accuracy is crucial.

- Mean Absolute Error (MAE)
MAE computes the average absolute difference between predicted and actual values. It treats all errors equally, making it more robust to outliers compared to MSE.

- Mean Squared Logarithmic Error (MSLE)
MSLE operates on the logarithm of predicted and actual values, measuring relative differences. It is useful when predicting values across varying scales and is less sensitive to outliers than MSE.

## Practical Implementation in TensorFlow/Keras
The repository includes practical examples using TensorFlow's Keras API to implement and evaluate these loss functions:

- Code Snippet

import tensorflow as tf
from tensorflow import keras

(Example model using MSE)
model = keras.Sequential([
    tf.keras.layers.Dense(100, activation='relu', input_shape=[len(train_features[0])]),
    tf.keras.layers.Dense(50, activation='relu'),
    tf.keras.layers.Dense(1)
])

model.compile(optimizer='adam',
              loss='mse',
              metrics=['mse'])

model.fit(train_features, train_labels, epochs=250, validation_split=0.1)

##Comparative Analysis

- MSE: Emphasizes larger errors due to squaring, suitable for tasks demanding precise accuracy.
- MAE: Treats all errors equally, robust to outliers, and easier to compute gradients.
- MSLE: Less sensitive to outliers, suitable for tasks with varying scales of target values

## Challenging, interesting, or exciting aspects of today's 

Today's assignment brought forth some intriguing challenges and learning opportunities. Exploring regression loss functions like MSE, MAE, and MSLE required me to dive into how each one measures prediction errors in different ways. Setting up these functions in TensorFlow and Keras was a bit of a puzzle, but it was satisfying to see how they influenced the performance of my neural network models

## Additional resources
1. Did you need to use tools like AI tools ChatGPT or Gemini to answer any of the questions or learn any of the concepts in this notebook? If  yes, state for which questions or concepts did you require Generative AI tools? 

No

2. If you answered "yes" to Question #1, which part of the answers are written by you, and which part of the answers are written by an AI tool? 

3. If you answered "yes" to Question #1, after using the AI tool to gain a better understanding of the material in this notebook, summarize your learnings here.

4. Did you use any other resources besides AI tools?

Mentor assistance
