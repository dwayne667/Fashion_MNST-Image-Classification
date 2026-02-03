# CSC-120
INTELLIGENT SYSTEMS

1. What is the Fashion MNIST dataset?
The Fashion MNIST dataset is a collection of 70,000 grayscale images of clothing items, each sized 28×28 pixels. It contains 60,000 training images and 10,000 test images, divided into 10 classes such as T-shirt/top, Trouser, Dress, Sneaker, and Ankle boot. It is commonly used as a benchmark dataset for image classification tasks and as a replacement for the original MNIST digits dataset.

2. Why do we normalize image pixel values before training?
We normalize image pixel values to scale them from the range 0–255 down to 0–1. This helps the neural network train faster and more efficiently by keeping input values small and consistent. Normalization also improves numerical stability and helps the optimizer converge more reliably during training.

3. List the layers used in the neural network and their functions.
Flatten layer: Converts the 2D image (28×28) into a 1D array so it can be processed by dense layers.
Dense (128 units, ReLU activation): A fully connected hidden layer that learns important features and patterns from the images.
Dense (10 units): The output layer that produces raw prediction scores (logits) for the 10 clothing classes.

4. What does an epoch mean in model training?
An epoch represents one complete pass of the entire training dataset through the neural network. During each epoch, the model updates its weights based on the loss calculated from the training data. Multiple epochs allow the model to gradually improve its accuracy.

5. Compare the predicted label and actual label for the first test image.
For the first test image, the predicted label matches the actual label (based on the output shown). This means the model correctly classified the image, indicating it learned useful features from the training data.

6. What could be done to improve the model’s accuracy?
The model’s accuracy could be improved by:
Adding more hidden layers or increasing the number of neurons
Using convolutional neural networks (CNNs) instead of a simple dense model
Training for more epochs
Applying regularization techniques such as dropout
