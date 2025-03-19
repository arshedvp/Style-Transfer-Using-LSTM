# Style Transfer using LSTM

This project demonstrates style transfer using Long Short-Term Memory (LSTM) networks. The model is trained to predict the next character in a sequence, allowing it to generate text in the style of the input data.

## Installation 🛠️

To get started with this project, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/HishamAbdulAsis/Style-Transfer-using-LSTM.git
    cd Style-Transfer-using-LSTM
    ```

2. **Install the required dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

## Usage 🚀

1. **Download the necessary files**:
    The notebook downloads the required input text and pre-trained model files using `wget`:
    ```python
    !wget https://raw.githubusercontent.com/GL3MON/inpLSTM/main/input.txt
    !wget https://github.com/GL3MON/inpLSTM/raw/main/LSTM_256.h5
    ```

2. **Run the notebook**:
    Open the `LSTMforSession1.ipynb` notebook in Jupyter or Google Colab and run all the cells to train and evaluate the model.

## Notebook Overview 📓

### Gathering Data 📊

The `gatheringData` function reads the input text file, converts it to lowercase, and returns the raw text.

### Pre-Processing Data 🔄

The `preProcessingData` function creates dictionaries to map characters to integers and vice versa. It tokenizes the text into sequences and splits the data into training and evaluation sets.

### Creating Model 🏗️

The `createModel` function defines an LSTM model with a specified number of units and dropout rate.

### Training Model 🏋️

The `trainingModel` function compiles and trains the model using categorical crossentropy as the loss function and Adam as the optimizer.

### Evaluation of Model 📈

The `evalModel` function evaluates the model using the evaluation split.

### Generate Predictions 🔮

The `predictSentences` function generates text predictions by processing the output vector of the LSTM model.

## Requirements 📦

- numpy
- tensorflow

