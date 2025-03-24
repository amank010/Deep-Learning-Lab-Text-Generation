# Text Generation using RNN and LSTM

This project demonstrates text generation using Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM) networks. The models are trained on a dataset of poems using two encoding methods: One-Hot Encoding and Trainable Embeddings. The performance of both models is compared based on their training loss and generated text quality.

---

##  Project Structure

```
- text_generation.py      # Main Python code for training and generating text
- poems-100.csv           # Dataset containing poems for training
- README.md               # Project documentation
- results/                # Directory to store results
  - onehot_rnn_loss.png   # Loss graph for One-Hot RNN
  - embedding_lstm_loss.png # Loss graph for Embedding LSTM
- generated_poems.txt     # Sample generated poems
```

---

## ⚙ Requirements

Make sure you have the following installed:
- Python 3.x
- PyTorch
- Matplotlib
- KaggleHub
- NumPy
- CSV

Install packages using:
```bash
pip install torch matplotlib numpy kagglehub
```

---

##  Dataset

- The dataset `poems-100.csv` contains a collection of poems used for training.
- It is automatically downloaded using KaggleHub. Ensure you have access to the Kaggle dataset.
- Update the Kaggle API key if required.

---

##  How to Run

1. Clone the repository:
```bash
git clone <repository_link>
cd <repository_name>
```

2. Run the code:
```bash
python text_generation.py
```

This will:
- Train both RNN and LSTM models using One-Hot Encoding and Trainable Embeddings.
- Generate sample poems using both models.
- Save the training loss graphs to the `results/` folder.
- Save the generated poems to `generated_poems.txt`.

---

##  Results

### 🔎 **Loss Graphs**
- **One-Hot RNN:** `results/onehot_rnn_loss.png`
- **Embedding LSTM:** `results/embedding_lstm_loss.png`

###  **Generated Poems**
- The generated poems using both models can be found in `generated_poems.txt`.
- The LSTM generally produces more coherent text compared to the RNN.

---

##  Performance Comparison

| Metric                 | One-Hot RNN      | Embedding LSTM      |
|-------------------------|------------------|----------------------|
| Training Time           | Faster            | Slower               |
| Loss Convergence        | Higher Loss       | Lower Loss           |
| Text Coherence          | Poor              | Good                 |
| Long-Term Dependencies  | Struggles         | Efficiently Handled  |

### **Observations:**
- The LSTM with Trainable Embeddings achieves lower loss and generates more fluent and meaningful text.
- The One-Hot RNN is faster in training but struggles with text coherence and long-term memory.
- Embedding LSTM requires more training time but provides significantly better results.

---

##  Conclusion

- LSTM models with Trainable Embeddings are recommended for tasks requiring natural language generation.
- RNNs with One-Hot Encoding may serve as a baseline model but are not ideal for complex text generation tasks.

---

## 🛠️ Author
- **AMAN**
- Roll No.: 2K22/CO/48
- GitHub: https://github.com/amank010/Deep-Learning-Lab-Text-Generation.git


