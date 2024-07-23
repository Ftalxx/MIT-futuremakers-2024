# Artificial Neural Networks

## Topics covered in today's module
* Introduction to Neural Networks
* Hyperparameters
* Forward Pass
* Backpropagation
* Computing accuracy

## Main takeaways from doing today's assignment

## Purpose
The primary goal here is to grasp the fundamental concepts of neural networks through hands-on implementation. By avoiding high-level abstractions, we gain insights into how data flows through the network, how weights are initialized and updated, and how activations affect predictions.

## Dataset
We use the MNIST dataset, a classic in the machine learning community for image classification. The dataset consists of grayscale images of handwritten digits along with their corresponding labels.

## Approach
Instead of leveraging TensorFlow, I opted to implement key functionalities manually using Python and NumPy. This decision allows for a clearer understanding of each step involved in training a neural network:

- Data Preparation: Loading the dataset, normalizing pixel values, and splitting into training and validation sets.

- Model Architecture: Defining the neural network architecture including input, hidden, and output layers. Weights are initialized and updated using basic matrix operations.

- Activation Functions: Implementing activation functions like Sigmoid and Softmax, crucial for introducing non-linearity and producing meaningful outputs.

- Forward Propagation: Calculating predictions by passing input data through the layers using matrix multiplication and activation functions.

- Backpropagation: Adjusting weights based on the error calculated from predictions and actual labels, ensuring the model learns from its mistakes.

- Training Loop: Iteratively refining the model through epochs, evaluating its performance on a validation set, and adjusting weights using Stochastic Gradient Descent (SGD).

## Insights Gained
Through this exercise, I gained a deeper appreciation for:

- Gradient Descent: Understanding how adjusting weights in the opposite direction of gradients reduces errors incrementally.

- Activation Functions: Seeing how Sigmoid and Softmax functions transform raw outputs into probabilities and enforce non-linearity.

- Matrix Operations: Realizing the efficiency and power of matrix operations in handling large-scale computations fundamental to neural networks.

## Challenging, interesting, or exciting aspects of today's assignment

Performance: Without GPU acceleration and optimized libraries, training times were longer compared to TensorFlow. Which was pretty interesting to consider.

## Additional resources
1. Did you need to use tools like AI tools ChatGPT or Gemini to answer any of the questions or learn any of the concepts in this notebook? If  yes, state for which questions or concepts did you require Generative AI tools? 

No

2. If you answered "yes" to Question #1, which part of the answers are written by you, and which part of the answers are written by an AI tool? 

3. If you answered "yes" to Question #1, after using the AI tool to gain a better understanding of the material in this notebook, summarize your learnings here.

4. Did you use any other resources besides AI tools?

Mentor assistance and stack overflow
