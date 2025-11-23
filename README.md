"""

# 🧠 Next Word Prediction Using LSTM

A deep learning project that predicts **the next word in a sentence** using an **LSTM-based language model** trained on Shakespeare’s _Hamlet_. It implements a complete NLP pipeline — from dataset preprocessing and sequence creation to model training, evaluation, and deployment via **Streamlit**.

---

## 🚀 Project Features

- LSTM architecture for next-word sequence prediction
- Trained on Shakespeare’s **_Hamlet_**
- End-to-end workflow: _preprocessing → training → evaluation → deployment_
- **Streamlit** web application for real-time word prediction
- **Early stopping** applied to minimize overfitting

---

## 📌 Tech Stack

| Component            | Technology                    |
| -------------------- | ----------------------------- |
| Programming Language | Python                        |
| Deep Learning        | TensorFlow / Keras            |
| NLP Tools            | Tokenizer, Embedding, Padding |
| Deployment           | Streamlit                     |
| Dataset              | Shakespeare — _Hamlet_        |

---

## 📂 Project Structure

📁 Next-Word-Prediction-LSTM  
│  
├── 📁 data  
│ └── hamlet.txt  
│  
├── 📁 notebooks  
│ └── model_training.ipynb  
│  
├── 📁 saved_model  
│  
├── streamlit_app.py  
├── requirements.txt  
└── README.md

---

## 🔧 How It Works

### 🔹 1. Data Preprocessing

- Load and clean raw text
- Tokenize text and convert words to integer indices
- Create input–output sequences for next-word prediction
- Pad sequences to uniform length for model input

### 🔹 2. Model Architecture

- **Embedding layer**
- **Two stacked LSTM layers**
- **Dense + Softmax output layer** to generate probability for the next word

### 🔹 3. Training

- Optimizer: `Adam`
- Loss function: `Categorical Cross-Entropy`
- Early stopping monitors validation loss to prevent overfitting

### 🔹 4. Evaluation

Assessed using multiple sentence prompts to determine prediction accuracy and linguistic coherence.

---

## 🌐 Streamlit Web App

Run locally:

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

Example:

```bash
 Input: To be or not to
 Output: be
```

---

## 📈 Results

The trained model demonstrates strong ability to auto-complete sentences and replicate Shakespeare-style language.

| Input                  | Predicted Next Word |
| ---------------------- | ------------------- |
| "The king shall never" | speak               |
| "My lord I have"       | done                |
| "To be or not to"      | be                  |

---

## 🛠️ Setup & Installation

```bash
git clone <your-repo-link>
cd <repo-name>
pip install -r requirements.txt
```

---

## 📌 Future Improvements

- Train on larger multi-author corpora
- Use **Bidirectional LSTM** / **Transformers** for improved accuracy
- Predict **multiple future words** instead of just one
- Export model & offer **REST API** deployment

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to open issues or submit pull requests 💡

---

## 📜 License

This project is licensed under the **MIT License**.
