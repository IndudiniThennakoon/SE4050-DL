# Deep Learning – Lab 5

## Comprehensive RNN and LSTM Model Implementation

**Objective:** Develop and evaluate various Recurrent Neural Network (RNN) architectures to handle different types of prediction tasks using sequential data. This includes:

1. **Basic RNN:** Implement a simple RNN to predict the next value in a small sequence of numbers. Explore how changing the number of hidden units and training parameters affects model performance.

2. **LSTM for Time-Series Forecasting:** Build and optimize an LSTM model to predict stock prices using historical data. Experiment with LSTM layer configurations, dropout rates, and training parameters to enhance forecasting accuracy.

3. **Sentiment Analysis with LSTM:** Apply an LSTM model for sentiment analysis on a text dataset (IMDB movie reviews). Compare the performance of bidirectional and unidirectional LSTM architectures and analyze their impact on model accuracy and F1-score.

In this task, you will gain hands-on experience with various RNN architectures, including basic RNNs and LSTMs, to address sequential data problems across different domains.


## 🚀 Tasks 1 : Understanding Basic RNN Architecture

**Objective:** Implement a simple RNN to predict the next value in a small sequence of numbers.

### 🏷️ Task :
- Upload the `Q1.ipynb` file to Jupyter Notebook (or Google Colab).
- Rename the `Q1.ipynb` file with your IT number (e.g., `ITxxxxxxQ1.ipynb`).
- Read the descriptions and instructions given in the notebook.
- Modify the `units` parameter in the `SimpleRNN` layer to see how the number of hidden units affects the model's ability to learn the sequence.
- Adjust the `epochs` and `batch_size` during training to optimize the model's learning process and performance.
- Analyze the resulting plot. If the predicted values deviate significantly from the actual values, experiment with different model configurations and training parameters to improve accuracy.
- Describe your observations. You can add a text cell and type your answers.

### 🚀 Task 2: Implementing LSTM for Time-Series Forecasting

**Objective:** Implement an LSTM model to predict stock prices using historical data.

### 🏷️ Task:
- Upload the `Q2.ipynb` file to Jupyter Notebook (or Google Colab).
- Upload the `google.csv` file to the root (content) directory of the VM.
- Rename the `Q2.ipynb` file with your IT number (e.g., `ITxxxxxxQ2.ipynb`).
- Modify the number of units in the LSTM layers and consider adding more layers or changing the dropout rate to see how these adjustments affect the model's performance.
- Adjust the `epochs` and `batch_size` during the training phase to optimize the model’s learning process and its ability to generalize.
- Examine the plot comparing predicted stock prices with actual prices. If the model’s predictions are inaccurate, experiment with different configurations and training parameters to achieve better results.
- Answer the following questions. (You can type your answers in a text cell):
  1. What is the purpose of normalizing the 'Close' prices before feeding them into the LSTM model?
  2. What is the purpose of the Dropout layer in the LSTM model?
  3. In the plot showing actual vs. predicted stock prices, what does it indicate if the predicted line closely follows the actual line?

## 🚀 Task 3: Sentiment Analysis using LSTM

**Objective:** Implement an LSTM model for sentiment analysis on a text dataset (IMDB movie reviews).

### 🏷️ Task:
- Upload the `Q3.ipynb` file to Jupyter Notebook (or Google Colab).
- Upload the `IMDB Dataset.csv` file to the root (content) directory of the VM.
- Rename the `Q3.ipynb` file with your IT number (e.g., `ITxxxxxxQ3.ipynb`).
- Modify the `output_dim` in the `Embedding` layer and the `units` in the `LSTM` layers. Consider adding dropout for regularization.
- Adjust the `epochs` and `batch_size` to observe how different training configurations impact the model’s performance.
- After training, review the accuracy and F1-score. If the scores are unsatisfactory, experiment with different model architectures, training configurations, and hyperparameters.
- In the above exercise, we used a bidirectional LSTM model:
  1. Compare the performance of the bidirectional LSTM with a unidirectional LSTM using the same dataset. (You will need to modify the model to unidirectional.)
  2. Analyze the impact of each architecture on model accuracy and F1-score. (You can use the same notebook and type your answers in a text cell.)


___________     
<sub><sup>📌 *documented by @IndudiniThennakoon 2024* </sup></sub>
