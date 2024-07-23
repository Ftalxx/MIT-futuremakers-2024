# Deep Learning and TensorFlow

## Topics covered in today's module
* Linear models in machine learning
* Introduction to TensorFlow
* Dataloaders
* Building a simple Neural Network

## Main takeaways from doing today's assignment
I explored the concepts behind Linear Regression:

- What does .score() indicate?
.score() computes the coefficient of determination (𝑅^2), showing how well the model predicts the target based on input data.

- What do reg.coef_ and reg.intercept_ represent?
reg.coef_ are the coefficients assigned to features, indicating their impact on the target.
reg.intercept_ is the bias term, representing the expected mean value of the target when all features are zero.

## Visualization
I visualized how the Linear Regression model attempts to separate the four classes in the XOR dataset using a line. This visualization highlighted the model's limitations in handling non-linear separations.

## Neural Network Modeling with TensorFlow
To explore more complex patterns in the XOR dataset, I used TensorFlow to build neural networks. Here's what I learned:

- Question 2
I compared a deeper neural network model to a simpler one:

Effect of adding layers and nodes on model performance?
Adding more layers and nodes generally improves the model's ability to learn complex patterns, potentially reducing loss and improving accuracy.

- Question 3
I experimented with adding layers incrementally to find optimal model performance:

Maximum number of layers for improved accuracy?
Increasing layers allows the network to capture deeper feature hierarchies, enhancing its ability to classify the XOR dataset accurately.

- Question 4
I discussed activation functions in the final layer of neural networks:

Why use sigmoid instead of softmax?
Sigmoid is suitable for binary classification tasks like ours, providing output probabilities between 0 and 1, ideal for distinguishing between two classes.

## Challenging, interesting, or exciting aspects of today's assignment
Overcoming obstacles such as overfitting and underfitting models provided valuable learning experiences. Troubleshooting errors and optimizing model performance taught me more than I had expected so now I can understand the concept better.

## Additional resources
1. Did you need to use tools like AI tools ChatGPT or Gemini to answer any of the questions or learn any of the concepts in this notebook? If  yes, state for which questions or concepts did you require Generative AI tools? 

No

2. If you answered "yes" to Question #1, which part of the answers are written by you, and which part of the answers are written by an AI tool? 

3. If you answered "yes" to Question #1, after using the AI tool to gain a better understanding of the material in this notebook, summarize your learnings here.

4. Did you use any other resources besides AI tools?

Stack Overflow
