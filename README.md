🧠 Next Word Prediction Using LSTM

A deep learning project that predicts the next word in a sentence using an LSTM-based language model trained on Shakespeare’s Hamlet. The project includes a full NLP pipeline — from data preprocessing and sequence generation to model training, evaluation, and deployment with Streamlit.

🚀 Project Features

Uses Long Short-Term Memory (LSTM) networks for sequence prediction

Trained on the full text of Shakespeare’s Hamlet

End-to-end workflow: preprocessing → training → evaluation → deployment

Streamlit web app for real-time prediction

Implements early stopping to reduce overfitting

📌 Tech Stack
Component	Technology
Programming Language	Python
Deep Learning	TensorFlow / Keras
NLP Tools	Tokenizer, Embedding, Padding
Deployment	Streamlit
Dataset	Shakespeare — Hamlet
📂 Project Structure
├── data/
│   └── hamlet.txt
├── notebooks/
│   └── model_training.ipynb
├── saved_model/
├── streamlit_app.py
├── requirements.txt
└── README.md

🔧 How It Works
1️⃣ Data Preprocessing

Load and clean raw text

Tokenize text and map each word to an index

Generate input–output word sequences

Pad sequences to uniform length

2️⃣ Model Architecture

Embedding layer

Two stacked LSTM layers

Dense layer with softmax for next-word probability

3️⃣ Training

Optimizer: Adam

Loss: Categorical Cross-Entropy

Early stopping to prevent overfitting

4️⃣ Evaluation

Tested on example inputs to measure prediction accuracy and sentence coherence.

🌐 Streamlit Web App

Run locally:

pip install -r requirements.txt
streamlit run streamlit_app.py


Enter any sentence and get the predicted next word in real time.
Example:

Input: To be or not to
Output: be

📈 Results

The trained model shows strong ability to auto-complete text and capture linguistic style of Shakespearean writing.
Example generations:

Input	Predicted Next Word
"The king shall never"	speak
"My lord I have"	done
"To be or not to"	be
🛠️ Setup & Installation
git clone <your-repo-link>
cd <repo-name>
pip install -r requirements.txt

📌 Future Improvements

Train on larger multi-author corpora

Use Bidirectional LSTM / Transformer for improved performance

Predict multiple future words instead of one

Add model export & API mode

🤝 Contributing

Contributions are welcome!
Feel free to open issues or submit pull requests 💡

📜 License

This project is licensed under the MIT License.

Contributions are welcome!
Feel free to open issues or submit pull requests 💡

📜 License

This project is licensed under the MIT License.
