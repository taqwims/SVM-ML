# report
Repositori ini merupakan implementasi analisis sentimen menggunakan Support Vector Machine (SVM) dengan data ulasan film. Model yang telah dilatih kemudian di-deploy melalui API berbasis Flask.

---

## Teknologi

- Python
- Scikit-learn
- Pandas
- Flask
- Pickle

---

## Cara Kerja

### 1. **Training Model (`svm_linear.py`)**
- Menggunakan dataset dari Cornell Movie Review Polarity v2.0.
- TF-IDF digunakan untuk ekstraksi fitur.
- Model dilatih dengan SVM (kernel linear).
- Evaluasi menggunakan `classification_report`.

### 2. **Menyimpan Model (`pickling.py`)**
- Menyimpan `vectorizer` dan `classifier_linear` ke file `.sav` menggunakan `pickle`.

### 3. **API untuk Prediksi (`classifier_flask.py`)**
- Menggunakan Flask untuk menyediakan endpoint `/sentiment`.
- Menerima teks via parameter `text`.
- Mengembalikan hasil prediksi sentimen (`positive` atau `negative`).


---
# SVM_sentiment_analysis

To find the sentiment(**positive/negative**) of the text data provided. This classifier model is implemented with **_SVM(kernel=linear)_**

# Install requirements

**pip install -r requirements.txt**

# End_point

sentiment

# Params

text

# Url

http://127.0.0.1:5000/sentiment?text="review_text"

# How to run

![flask app](https://github.com/Vasistareddy/sentiment_analysis/blob/master/data/flask_app.gif)
