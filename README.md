# Deep-Learning-Lab-Text-Generation
Text Generation
## Results
- The training loss graph for the One-Hot RNN model is available at `results/onehot_rnn_loss.png`.
- The training loss graph for the Embedding LSTM model is available at `results/embedding_lstm_loss.png`.
- Generated poems from both models can be found in `generated_poems.txt`.

### Observations
- The LSTM model generally converges faster and achieves lower loss compared to the One-Hot RNN model.
- The One-Hot RNN model struggles to capture long-term dependencies, while the LSTM model generates more coherent poetry.
- Training time for LSTM is longer but more effective in generating readable text.
