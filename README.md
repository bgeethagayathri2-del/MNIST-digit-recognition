# MNIST Handwritten Digit Recognition

Recognizes handwritten digits (0 to 9) using deep learning, and compares a simple neural network with a CNN.

- **Dataset:** MNIST (60,000 training images and 10,000 test images, 28x28 pixels)
- **Models:** Simple neural network (2 hidden layers) and Convolutional Neural Network (CNN)
- **Training:** 5 epochs each, using Keras (TensorFlow)
- **Results:**

| Model | Test accuracy | Wrong out of 10,000 |
|---|---|---|
| Simple Neural Network | 0.9774 | about 226 |
| CNN | 0.9898 | about 102 |

- **Conclusion:** The CNN performed better, reaching 98.98% test accuracy against 97.74% for the simple network, and it made less than half as many mistakes. A CNN looks at small patches of the image (such as edges and curves), so it understands the shape of a digit better than a simple network that only sees a flat list of pixels. The simple network's training accuracy (98.5%) kept rising while its validation loss stopped improving, which is an early sign of overfitting. The CNN's results were steadier.

## How to run
Open `MNIST_digits.ipynb` in Google Colab and click Run all.
