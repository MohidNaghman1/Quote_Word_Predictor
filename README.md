# Quote Completion using LSTM

This project is a deep learning-based text generation model that predicts the next five words of a given quote. The model uses **Tokenization**, **Padding**, and an **LSTM (Long Short-Term Memory) model** for text generation.

## Features
- Tokenizes input text
- Uses padding to ensure consistent input length
- Predicts the next words using an LSTM model
- Generates a completed quote based on the given input

## Technologies Used
- Python
- TensorFlow/Keras
- NumPy
- Pickle (for saving and loading the tokenizer)

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/quote-completion-lstm.git
cd quote-completion-lstm
```

### 2. Install Dependencies
```bash
pip install tensorflow numpy
```

### 3. Download the Pretrained Model & Tokenizer
Make sure you have the trained model (`quote_model.h5`) and tokenizer (`tokenizer.pkl`) in the project directory.

## Usage
### Running the Script
```bash
python predict_quote.py
```
You will be prompted to enter the beginning of a quote, and the script will generate the next five words based on the trained model.

## How It Works
1. The input text is tokenized using a pre-trained tokenizer.
2. The tokenized sequence is padded to match the required input length.
3. The LSTM model predicts the next word based on the input.
4. The generated word is appended to the input, and the process repeats for five words.

## Example Output
**Input:** "The truth is"

**Output:** "The truth is always hard to accept"

## Future Improvements
- Train the model on a larger dataset for better predictions.
- Develop a web interface for user interaction.

