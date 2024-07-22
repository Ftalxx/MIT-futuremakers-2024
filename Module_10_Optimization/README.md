# Optimization

## Topics covered in today's module
* Gradient Descent
* Stochastic Gradient Descent
* Batch gradient Descent
* Hyperparameter Tuning

## Main takeaways from doing today's assignment

In this repository, I explored various optimization algorithms used in deep learning, focusing on their roles, implementations in TensorFlow 2.0, and their application to training neural networks effectively.

## Optimization Algorithms

What is Optimization?
Optimization involves finding the best solution from a set of options based on a defined metric. In deep learning, this metric is typically a loss function that measures the difference between predicted and actual outcomes.

How Optimization is Used in Machine Learning:
Optimization algorithms are crucial in machine learning to adjust model parameters iteratively. The goal is to minimize the loss function, improving the model's predictive accuracy.

Optimizers and Loss Functions:
Optimizers adjust model parameters to minimize the loss function. They work in tandem with the loss function, ensuring the model learns efficiently by updating parameters based on the gradient of the loss.

Gradient Descent:
Gradient descent is a fundamental optimization algorithm in deep learning. It updates model parameters in the opposite direction of the gradient of the loss function, scaled by a learning rate.

## Variants of Gradient Descent
  
Batch Gradient Descent (BGD): Uses the entire dataset to compute the gradient.
Stochastic Gradient Descent (SGD): Computes the gradient using a single random data point.
Mini-batch Gradient Descent: Computes the gradient using a small subset (mini-batch) of the dataset.
Advantages of SGD over BGD
SGD is preferred over BGD in scenarios where:
  * The dataset is large and cannot fit into memory.
  * Faster computations are required.
  * Frequent updates are needed for quicker convergence.
  * Exploration of better solutions in non-convex problems is desired.
  * Implementing Optimization Algorithms in TensorFlow 2.0

## Practical Example: Training a Multi-Layer Perceptron (MLP) on FashionMNIST
I used TensorFlow's Keras API to train a simple MLP on the FashionMNIST dataset. Here's a summary of the process:

Loading and Preprocessing Data: Loaded FashionMNIST dataset, normalized pixel values, and prepared batches.

Building the MLP: Defined a simple MLP architecture using Keras Sequential API.

Training with Different Optimizers:
SGD: Standard stochastic gradient descent.
SGD with Momentum: Improved SGD using momentum for faster convergence.
RMSProp: Optimizer suitable for recurrent neural networks (RNNs) and reinforcement learning (RL).
Adam: Adaptive moment estimation optimizer.
SGD with Learning Rate Decay: SGD with a decaying learning rate to stabilize training.

From the results, Adam generally performed well across different scenarios, while SGD and SGD with momentum also showed competitive performance.

## Conclusion

Optimization algorithms play a critical role in training deep learning models effectively. Choosing the right optimizer depends on the specific problem, dataset size, and computational resources available

## Challenging, interesting, or exciting aspects of today's assignment

Implementing AdaGrad in Keras and conducting a comparative analysis of optimization algorithms required overcoming technical challenges related to understanding the method, integrating it into a deep learning framework, debugging implementation issues, conducting rigorous experimentation, and interpreting the results accurately.

## Additional resources

1. Did you need to use tools like AI tools ChatGPT or Gemini to answer any of the questions or learn any of the concepts in this notebook? If  yes, state for which questions or concepts did you require Generative AI tools? 

Yes, I did use AI.

2. If you answered "yes" to Question #1, which part of the answers are written by you, and which part of the answers are written by an AI tool?

I tried to get help on question 4 for the structure of the code but it was too complex for the AI. I requested help from my mentor instead.

4. If you answered "yes" to Question #1, after using the AI tool to gain a better understanding of the material in this notebook, summarize your learnings here.

Not necessarily.

6. Did you use any other resources besides AI tools?

No.
