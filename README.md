
# 🏷️ NOTE:
- The answer sheets, including screenshots for Task 1 and Task 2, are in the `Task 01 Answer.txt` and `Task 02 Answer.txt` files.
- The modified notebooks (`Backprop.ipynb`, `NN_sample.ipynb`, `MLP_with_MNIST_dataset.ipynb`) are available in the repository.


# Deep Learning – Lab 2

## Overview
In this lab, you will work with Jupyter notebooks or Google Colab to complete various tasks related to deep learning. Follow the instructions below to perform the exercises and submit your work.

## Instructions

### 1. Backpropagation Notebook
- Upload the `Backprop.ipynb` file to Jupyter Notebook or Google Colab.
- Understand the code and increase the number of iterations (epochs) to see if it improves the prediction accuracy.
- **Note:** You may need to copy the `image.png` file to the home directory for the notebook to function correctly.

### 2. Neural Network Sample Notebook
- Upload the `NN_sample.ipynb` file to Jupyter Notebook or Google Colab.
- Add the following text and code cells to the notebook and run it again:
  - **Text Cell:**
    ```markdown
    Now, let's try out several hidden layer sizes. 4.6 - Tuning hidden layer size (optional/ungraded exercise)¶
    ```
  - **Code Cell:**
    ```python
    # This may take about 2 minutes to run
    hidden_layer_sizes = [1, 2, 3, 4, 5, 20, 50]
    for i, n_h in enumerate(hidden_layer_sizes):
        parameters = nn_model(X, Y, n_h, num_iterations = 5000)
        # plot_decision_boundary(lambda x: predict(parameters, x.T), X, Y)
        predictions = predict(parameters, X)
        accuracy = float((np.dot(Y,predictions.T) + np.dot(1-Y,1-predictions.T))/float(Y.size)*100)
        print("Accuracy for {} hidden units: {} %".format(n_h, accuracy))
    ```
- **Questions:**
  1. What happens when the number of hidden nodes increases?
  2. Can you explain the pattern of the accuracy when the hidden nodes increase?
- **Note:** Copy the `planar_utils.py` and `testCases.py` files to the home directory.

### 3. MLP with MNIST Dataset Notebook
- Run the `MLP_with_MNIST_dataset.ipynb` file using Jupyter Notebook or Google Colab.
- Improve the test accuracy of the model by changing the hyperparameters.
- Add L1 and L2 regularization terms to the model and retrain it.
- Visualize class-wise test dataset performance using a confusion matrix.

### 4. Optional Exercise
- Open the [neural network playground](https://playground.tensorflow.org/) and experiment with different hyperparameters.
- Observe if L1 and L2 regularization can be used to reduce overfitting.

___________     
<sub><sup>📌 *documented by @IndudiniThennakoon 2024* </sup></sub>

