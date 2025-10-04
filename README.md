## 🧠 Next Word Prediction Using LSTM

A deep learning project that predicts the next word in a given sentence using an **LSTM (Long Short-Term Memory)** model.
This project demonstrates the application of **Recurrent Neural Networks (RNNs)** in **Natural Language Processing (NLP)** by learning from the text of *Shakespeare’s Hamlet*.

---

## 📘 Project Overview

This project builds a next-word prediction model using an **LSTM-based neural network** trained on literary text.
By analyzing word sequences, the model learns contextual relationships and predicts the most probable next word.

---

## 🧩 Workflow

### 1️⃣ Data Collection

* The dataset used is **Shakespeare’s “Hamlet”**, a classic English text.
* The complexity and richness of the text make it ideal for learning contextual word patterns.

### 2️⃣ Data Preprocessing

* The text is **tokenized** using Keras Tokenizer.
* Tokens are converted into sequences and **padded** for uniform length.
* Data is split into **training and validation** sets.

### 3️⃣ Model Building

* An **Embedding layer** converts tokens into dense vectors.
* Two **LSTM layers** capture long-term dependencies.
* A **Dense output layer** with **Softmax activation** predicts the next word.

Model summary:

```
Embedding → LSTM → LSTM → Dense (Softmax)
```

### 4️⃣ Model Training

* The model is trained on prepared sequences.
* **EarlyStopping** is implemented to avoid overfitting.
* Training progress is monitored via **validation loss**.

### 5️⃣ Model Evaluation

* The trained model is evaluated using example sentences.
* The accuracy of next-word predictions is tested on unseen sequences.

### 6️⃣ Deployment

* A **Streamlit Web App** allows users to:

  * Enter a sentence.
  * Get the **predicted next word** instantly.
* The app uses the trained model (`next_word_lstm.h5`) and tokenizer (`tokenizer.pickle`).

---

## 📂 Project Structure

```
Next_Word_Prediction/
│
├── main.py                # Streamlit application for prediction
├── next_word_lstm.h5      # Trained LSTM model
├── tokenizer.pickle       # Saved tokenizer for text encoding
├── requirements.txt       # List of dependencies
└── .venv/                 # Virtual environment (optional)
```

---

## 🧠 Technologies Used

* **Python 3.x**
* **TensorFlow / Keras**
* **NumPy**
* **Streamlit**
* **Pickle**

---

## 🚀 How to Run

1️⃣ **Clone this repository**

```bash
git clone https://github.com/your-username/Next_Word_Prediction.git
cd Next_Word_Prediction
```

2️⃣ **Install dependencies**

```bash
pip install -r requirements.txt
```

3️⃣ **Run the Streamlit app**

```bash
streamlit run main.py
```

4️⃣ **Use the Web Interface**

* Enter a phrase like:

  > "To be or not to"
* Get output:

  > Predicted next word → *"be"*

 <img width="1545" height="860" alt="image" src="https://github.com/user-attachments/assets/e6b0cb5f-7ed8-4170-a275-a4cf47982e7d" />


---

## 📈 Results

The model achieves meaningful predictions on literary text, demonstrating the capability of LSTM networks to understand linguistic context.

---

## 🧑‍💻 Author

**Virendra Badgotya**
B.Tech in Electrical Engineering | SVNIT Surat
🔗 [GitHub](https://github.com/vir123-devf) | [LinkedIn](https://www.linkedin.com/in/virendra-badgotya-ai/)

---

Would you like me to include an **example screenshot section** (for your Streamlit app interface) in the README as well? It can make your GitHub page look more appealing.
