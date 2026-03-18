# fake-news-detection-Lstm
Binary text classification model to detect fake news using LSTM, NLP preprocessing, and TensorFlow/Keras. Achieves ~95% accuracy on news article dataset.

# 📰 Fake News Detection Using LSTM

A deep learning project that detects fake news articles using Natural Language Processing (NLP) and Long Short-Term Memory (LSTM) neural networks.

---

## 🧠 Overview

With the rapid spread of misinformation online, detecting fake news has become a critical challenge. This project builds a binary text classification model that automatically classifies news articles as **Real** or **Fake** using an LSTM-based deep learning approach.

---

## 🚀 Tech Stack

| Category | Tools / Libraries |
|---|---|
| Language | Python |
| Deep Learning | TensorFlow, Keras |
| NLP | NLTK, PorterStemmer, Stopwords |
| ML Utilities | Scikit-learn |
| Data Handling | Pandas, NumPy |
| Model Architecture | Embedding → LSTM → Dense (Sigmoid) |

---

## 📂 Dataset

- **File:** `News.csv`
- **Columns:** `News Title`, `News Text`, `Class`
- **Target:** Binary classification — `0` (Fake) / `1` (Real)

---

## ⚙️ How It Works

1. **Data Preprocessing**
   - Removed null values
   - Applied text cleaning using Regex
   - Lowercased and stemmed words using PorterStemmer
   - Removed English stopwords using NLTK

2. **Text Encoding**
   - Used One-Hot Encoding and Keras Tokenizer
   - Vocabulary size: top 10,000 most frequent words
   - Padded sequences to fixed length of 20 tokens

3. **Model Architecture**
   ```
   Embedding Layer (vocab_size → 40 dimensions)
        ↓
   LSTM Layer (100 units)
        ↓
   Dense Layer (1 unit, Sigmoid activation)
   ```

4. **Training**
   - Loss: Binary Crossentropy
   - Optimizer: Adam
   - Epochs: 10
   - Batch Size: 64
   - Train/Test Split: 67% / 33%

5. **Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report (Precision, Recall, F1-Score)

---

## 📊 Results

| Metric | Score |
|---|---|
| Accuracy | ~94–96% (based on training run) |
| Loss Function | Binary Crossentropy |
| Evaluation | Confusion Matrix + Classification Report |

---

## 🔧 How to Run

1. Open the notebook in Google Colab or Jupyter Notebook
2. Upload the `News.csv` dataset
3. Run all cells sequentially
4. View accuracy and classification report at the end

[![Open In Colab](https://colab.research.google.com/drive/1htl07oJyUHoWi1QSa0XrwfNzOZJZSRdG?usp=sharing)

---

## 📁 Project Structure

```
fake-news-detection-lstm/
│
├── Fake_News_Detection_Using_LSTM.ipynb   # Main notebook
├── News.csv                                # Dataset
└── README.md                              # Project documentation
```

---

## 👨‍💻 Author

**Prashant Kumar Rai**  
B.Tech (CS) | M.Tech (Computer Engineering) — SGSITS Indore  
[LinkedIn]( www.linkedin.com/in/prashantkumarrai8788 ) • [GitHub]( https://github.com/raiprashantmittal )

