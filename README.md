# Handwritten Digit Classifier

A neural network that recognizes handwritten digits (0 to 9), built from scratch with NumPy: forward propagation, backpropagation, a regularized cost function, gradient descent and a numerical gradient check. No ML framework is used to build or train the network (scikit-learn only splits the data).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/phdaccache/handwritten-digit-classifier/blob/main/handwritten_digit_classifier.ipynb)

## Results

| Run | Result |
|---|---|
| Trained on all 5,000 images | 94.36% training accuracy |
| 60/20/20 split | 3.43% train, 8.5% validation, 9.3% test error |
| λ chosen on the validation set | best λ = 0.01, 9.4% test error |

## Running it

Open it in Colab with the badge above and run all cells. The data loads from two public Google Sheets, so there is nothing to download.

The notes inside the notebook are in Portuguese. This was a course project (MS571, second semester of 2022).
