# Next_Word_Prediction_LSTM
 This repository contains code for a simple next-word prediction model built using LSTM (Long Short-Term Memory) layers in TensorFlow/Keras. The project includes a Streamlit-based web app to demonstrate the functionality of the trained model.  

## Overview

The model is created and trained to predict the next word in a sequence based on input text. It is trained on a limited dataset for 20 epochs as a practice exercise to understand the workflow of text generation using LSTM.

### Key Features

- **Embedding Layer**: Encodes the input text sequences into dense vector representations.
- **Two LSTM Layers**: Extracts sequential dependencies from the text.
- **Dropout Layer**: Prevents overfitting during training.
- **Dense Output Layer**: Predicts the next word from the vocabulary using softmax activation.
- **Streamlit Integration**: Provides a user-friendly interface for next-word prediction.
- **Tokenizer Integration**: Preprocesses input text into sequences for prediction.
- **Model Loading**: Loads a pre-trained LSTM model (`next_word_lstm.h5`) for next-word prediction.
- **Tokenizer Loading**: Utilizes a pre-saved tokenizer (`tokenizer.pickle`) to preprocess and tokenize input text sequences.
- **Sequence Padding**: Ensures input sequences are padded to the correct length using `pad_sequences` for compatibility with the LSTM model.
- **Next Word Prediction Functionality**: Implements logic to predict the next word by processing user input and generating predictions using the trained model.
- **Streamlit Integration**: Provides a user-friendly interface where users can input text and get real-time predictions.

## Requirements

To run this project, you need the following:

- Python 3.7+
- TensorFlow
- Streamlit
- Numpy
- Pickle

Install the required dependencies using:
```bash
pip install tensorflow streamlit numpy
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/next-word-prediction.git
   cd next-word-prediction
   ```

2. Make sure the pre-trained model (`next_word_lstm.h5`) and tokenizer file (`tokenizer.pickle`) are in the project directory.

3. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

4. Open the local Streamlit server in your browser (usually at `http://localhost:8501`).

5. Enter a sequence of words and click "Predict Next Word" to see the model's prediction.

## Limitations

- **Limited Training**: The model was trained for only 20 epochs as a practice exercise, so its accuracy might not be optimal.
- **Dataset**: The vocabulary and context are restricted to the dataset used during training.


## Future Improvements

- Train the model on a larger dataset and for more epochs to improve accuracy.
- Implement attention mechanisms for better context understanding.
- Add support for multi-word predictions.


