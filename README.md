# Handwritten Digit Classifier

A neural network that recognizes handwritten digits (0 to 9), built from scratch with NumPy: forward propagation, backpropagation, a regularized cost function, gradient descent and a numerical gradient check. No ML framework is used to build or train the network (scikit-learn only splits the data).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/phdaccache/handwritten-digit-classifier/blob/main/handwritten_digit_classifier.ipynb)

## Results

| Run | Result |
|---|---|
| Trained on all 5,000 images | 94.36% training accuracy |
| 60/20/20 split | 3.43% train, 8.5% validation, 9.3% test error |
| λ chosen on the validation set | best λ = 0.01, 9.4% test error |

## What's in the notebook

1. **Data:** 5,000 handwritten digits, each a 20x20 grayscale image (400 inputs).
2. **The network:** every function written by hand. 400 inputs, 25 hidden units, 10 outputs, sigmoid activations.
3. **Gradient check:** backpropagation matches the numerically computed gradient to about 1e-9.
4. **Training:** the images it gets wrong, and what each hidden unit learned.
5. **Evaluation:** train, validation and test errors.
6. **Tuning:** choosing λ automatically, and a learning curve.

## Running it

Open it in Colab with the badge above and run all cells. The data loads from two public Google Sheets, so there is nothing to download. A full run takes about 1.5 to 2 hours on Colab's free tier, mostly the λ search and the learning curve, because backpropagation goes through the examples one at a time.

The notes inside the notebook are in Portuguese. This was a course project (MS71, second semester of 2022).
