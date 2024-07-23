# Convolution Neural Network

## Topics covered in today's module
* Convolution neural network components
* Visualizing kernels
* Visualizing feature maps
* Pooling
* Dropout
* Batch norm

## Main takeaways from doing today's assignment

## Convolutional Neural Networks (CNNs)
CNNs are inspired by the biological visual processing in animals and humans. They use a series of convolutional layers to extract features from input images. Each convolutional layer applies a set of filters to the input image, which helps detect patterns and features at different levels of abstraction.

## CNN Components
A typical CNN consists of convolutional layers, activation functions (often ReLU), pooling layers (e.g., max pooling), and fully connected layers. These components work together to progressively learn hierarchical representations of the input data.

## Fashion MNIST Dataset
The Fashion MNIST dataset is a popular benchmark in the machine learning community, serving as a replacement for the original MNIST dataset. It consists of grayscale images of clothing items belonging to 10 different classes. Each image is 28x28 pixels.

## Data Preparation
Before training a CNN model, it's essential to preprocess the data. This includes loading the dataset, dividing it into training and testing sets, and normalizing the pixel values. Normalization scales the pixel values from 0-255 to a range of 0-1, which helps the model converge faster during training.

## Model Architecture
We built a basic CNN model using TensorFlow/Keras:

Code Snippet

model = tf.keras.models.Sequential([
  tf.keras.layers.Conv2D(32, (3,3), activation='relu', input_shape=(28, 28, 1)),
  tf.keras.layers.MaxPooling2D(2, 2),
  tf.keras.layers.Conv2D(32, (3,3), activation='relu'),
  tf.keras.layers.MaxPooling2D(2, 2),
  tf.keras.layers.Flatten(),
  tf.keras.layers.Dense(128, activation='relu'),
  tf.keras.layers.Dense(10, activation='softmax')
])

## Training the Model

The model is compiled with an optimizer (Adam), loss function (sparse categorical cross-entropy), and metrics (accuracy):

Code Snippet

model.compile(optimizer='adam', loss='sparse_categorical_crossentropy', metrics=['accuracy'])
model.fit(training_images, training_labels, epochs=5)

## Visualizing Filters and Feature Maps

After training, we can visualize the learned filters and feature maps to understand what the network has learned:

- Filters: Filters (or kernels) in convolutional layers detect various patterns like edges or textures. Visualizing filters helps interpret the learned representations.

- Feature Maps: Feature maps are the outputs of convolutional layers and show how different parts of the input are activated by each filter. They help visualize what the network focuses on as it processes an image.

## Overfitting and Regularization
- Overfitting can occur when a model memorizes the training data and fails to generalize to new data. Techniques like dropout and batch normalization are used for regularization:

- Dropout: Randomly disables neurons during training to prevent reliance on specific features and improve generalization.

- Batch Normalization: Normalizes the inputs to each layer, stabilizing the learning process and reducing internal covariate shift.

## Challenging, interesting, or exciting aspects of today's assignment

Working with real-world image data and seeing the direct application of CNNs in classifying different types of clothing items was engaging. It bridged theoretical knowledge with practical implementation,

## Additional resources
1. Did you need to use tools like AI tools ChatGPT or Gemini to answer any of the questions or learn any of the concepts in this notebook? If  yes, state for which questions or concepts did you require Generative AI tools?

No, I did not use AI

3. If you answered "yes" to Question #1, which part of the answers are written by you, and which part of the answers are written by an AI tool? 

4. If you answered "yes" to Question #1, after using the AI tool to gain a better understanding of the material in this notebook, summarize your learnings here.

5. Did you use any other resources besides AI tools?

I used Stack Overflow
