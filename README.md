Perfect — now that I can clearly see your **exact GitHub folder structure**, here is a clean, simple, accurate **README.md** written specifically for *your repo*.

No exaggerations, no over-claims — just straightforward and modest.

---

# 📩 SMS Spam Classification

This project is a simple machine-learning implementation for classifying SMS messages as **spam** or **not spam**.
It contains two main parts:

1. **Training Notebook** – where the dataset is explored, cleaned, and the model is trained.
2. **Streamlit Application** – a minimal UI that loads the trained model and predicts spam/ham for user-entered text.

---

## 📁 Project Structure

```
sms-spam-classification/
│
├── sms-spam-detection.ipynb      # Notebook: preprocessing, EDA, model training
├── spam.csv                      # Dataset used for training
│
└── sms-spam-classification/      # Streamlit app folder
    ├── app.py                    # Streamlit UI for prediction
    ├── model.pkl                 # Saved trained model
    └── vectorizer.pkl            # Saved TF-IDF vectorizer
```

---

## 🧠 What the Project Does

### **Model & Preprocessing**

The notebook performs basic NLP steps:

* Lowercasing
* Tokenization
* Removing stopwords
* Removing punctuation
* Stemming using PorterStemmer
* TF-IDF vectorization
* Training a **Multinomial Naive Bayes** classifier

The trained model and vectorizer are saved as `.pkl` files.

### **Performance**

During training, the model achieved approximately:

* **Accuracy:** ~0.97
* **Precision:** ~0.97

(Values may vary based on retraining.)

---

## ▶️ Running the Streamlit App

Go into the Streamlit folder:

```sh
cd sms-spam-classification/sms-spam-classification
```

If using a virtual environment, activate it.
Then run:

```sh
streamlit run app.py
```

This opens the UI where you can enter a message and check if it's spam.

---

## 📊 Notebook Features

Inside **sms-spam-detection.ipynb**, you will find:

* Text preprocessing
* Dataset cleaning
* Spam/Ham WordClouds
* Bar plots of most common spam words
* Model training, evaluation, and saving

---

## 📝 Notes

* The notebook and the Streamlit app are separate for clarity.
* If you retrain the model, make sure to update `model.pkl` and `vectorizer.pkl` inside the Streamlit folder.
* This project is intended for learning NLP basics and creating a simple ML web app.

---

