# Text Prediction and Correction for Chat Messages

This repository demonstrates RNN, LSTM, and GPT models for text prediction and correction, designed for short-form chat messages in a simulator environment.

## Features
- RNN and LSTM models built with TensorFlow/Keras.
- GPT model using Hugging Face’s DistilGPT-2.
- Simulator for real-time text prediction and correction.
- Optimized for low latency (<50ms) and lightweight deployment.

## Setup
1. Clone the repo: `git clone https://github.com/jasserezzi/text-predictor`
2. Install dependencies: `pip install tensorflow transformers nltk`
3. Run the simulator: `python simulator.py`

## Example
Input: "hello how are"
- RNN: "you"
- LSTM: "you"
- GPT: "you doing"
Corrected: "hello how are you"

## Files
- `rnn_model.py`: Simple RNN for next-word prediction.
- `lstm_model.py`: LSTM with improved dependency handling.
- `gpt_model.py`: Fine-tuned DistilGPT-2 for prediction/correction.
- `simulator.py`: Integrates models for real-time use.
- `chat_data.txt`: Sample dataset.

## Results
- RNN Accuracy: ~65% (top-3)
- LSTM Accuracy: ~77% (top-3)
- Latency: ~30ms (CPU)

Explore the code and feel free to reach out for collaboration!
