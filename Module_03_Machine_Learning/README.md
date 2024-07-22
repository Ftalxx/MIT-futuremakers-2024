# Machine Learning

## Topics covered in today's module

* Introduction to Machine Learning
* Machine learning with Scikit-learn
* Decision Trees
* Linear Regression
* Random Forests

## Main takeaways from doing today's assignment

Machine learning is a fascinating field within artificial intelligence (AI) where systems learn and improve from data without explicit programming. It enables tasks like classification, regression, and clustering based on patterns inferred from data.

## Types of Machine Learning
- Supervised Learning: This method learns from labeled data, predicting outcomes based on input-output pairs. It includes tasks such as regression and classification.

- Unsupervised Learning: Here, the system learns from unlabeled data, uncovering patterns and structures without predefined outputs. 

- Semi-supervised Learning: This approach combines labeled and unlabeled data for training, balancing both structured guidance and broader data insights.

- Reinforcement Learning: Learning occurs through trial-and-error interactions with an environment, receiving rewards for actions leading to desired outcomes.

## Using Scikit-Learn for Machine Learning
Scikit-Learn is my go-to Python library for machine learning tasks, offering tools for model building, data preprocessing, and performance evaluation. It integrates seamlessly with other data handling libraries like NumPy, SciPy, and Pandas.

## Practical Example: Iris Dataset Visualization and Decision Tree Classification
One classic example is the Iris dataset, which I used to visualize and classify using Scikit-Learn:

Data Visualization: I plotted features such as sepal length, sepal width, petal length, and petal width using Matplotlib to gain insights into the dataset.

Decision Tree Classification: Leveraging Scikit-Learn's DecisionTreeClassifier, I built a model to classify Iris species based on these features.

## Decision Trees vs. Random Forests
Decision Trees: These are single-tree models that can overfit but provide transparent decision paths based on feature splits.

Random Forests: As an ensemble learning method, Random Forests combine multiple decision trees to reduce overfitting and improve accuracy through averaging predictions.

## Code Implementation

from sklearn.datasets import load_iris
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import train_test_split

- Load Iris dataset
iris = load_iris()
X = iris.data
y = iris.target

- Train a Decision Tree Classifier
tree = DecisionTreeClassifier()
tree.fit(X, y)

- Train a Random Forest Classifier
forest = RandomForestClassifier(n_estimators=100, random_state=42)
forest.fit(X, y)

## Challenging, interesting, or exciting aspects of today's assignment

It has been interesting to learn about simple machine learning. This is the first time I've encountered the idea that AI is deeply rooted in mathematics and statistics, particularly in how algorithms learn from data patterns to make predictions or decisions. Understanding the foundational concepts like supervised learning, where models are guided by labeled data to predict outcomes, and unsupervised learning, where algorithms uncover patterns without predefined labels, has been eye-opening.

## Additional resources
1. Did you need to use tools like AI tools ChatGPT or Gemini to answer any of the questions or learn any of the concepts in this notebook? If  yes, state for which questions or concepts did you require Generative AI tools? 

No

2. If you answered "yes" to Question #1, which part of the answers are written by you, and which part of the answers are written by an AI tool? 

3. If you answered "yes" to Question #1, after using the AI tool to gain a better understanding of the material in this notebook, summarize your learnings here.

4. Did you use any other resources besides AI tools?

Yes, Sklearn documentation. https://scikit-learn.org/stable/modules/tree.html
