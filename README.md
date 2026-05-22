# 🎵📈 Viral Content Classification using Machine Learning

## 📌 Projct Overview

Proyek ini bertujuan untuk melakukan klasifikasi apakah suatu konten video pendek termasuk **viral** atau **tidak viral** menggunakan metode Machine Learning.

Dataset yang digunakan berasal dari platform **YouTube Shorts** dan **TikTok Trends 2025**. Proses klasifikasi dilakukan menggunakan dua algoritma, yaitu:

* **Logistic Regression**
* **Random Forest**

Evaluasi model dilakukan menggunakan:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## 📂 Dataset

Sumber dataset: Kaggle
Nama dataset: **YouTube Shorts and TikTok Trends 2025**

Dataset terdiri dari sekitar **48.000 data** dengan berbagai fitur terkait performa dan interaksi konten media sosial.

### Contoh fitur:

* likes
* comments
* shares
* duration_sec
* avg_watch_time_sec
* completion_rate
* category
* platform
* genre
* upload_hour
* traffic_source

---

## 🎯 Problem Formulation

Proyek ini termasuk ke dalam **Supervised Learning** dengan tipe **Binary Classification**.

Target klasifikasi:

* `1` → Viral
* `0` → Tidak Viral

Variabel target (`viral`) dibuat menggunakan nilai median dari jumlah views:

* views > median → viral
* views ≤ median → tidak viral

Pendekatan ini digunakan agar distribusi data menjadi lebih seimbang dan model tidak bias terhadap salah satu kelas.

---

## ⚙️ Tahap Preprocessing

Tahapan preprocessing yang dilakukan meliputi:

* Data cleaning
* Menghapus fitur yang tidak relevan
* Menghindari data leakage
* One-hot encoding
* Feature scaling menggunakan `StandardScaler`
* Train-test split (80:20)

---

## 🤖 Models Used

### 1. Logistic Regression

Model klasifikasi sederhana yang digunakan sebagai baseline model untuk memprediksi probabilitas konten viral.

### 2. Random Forest

Model ensemble berbasis decision tree yang digunakan untuk menangkap pola data yang lebih kompleks.

---

## 📊 Hasil Evaluasi

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 90.3%    |
| Random Forest       | 90.1%    |

Kedua model menunjukkan performa yang baik dan stabil berdasarkan metrik:

* Precision
* Recall
* F1-Score

---

## 📈 Exploratory Data Analysis (EDA)

EDA dilakukan untuk:

* Melihat distribusi target
* Melihat korelasi antar fitur
* Mendeteksi outlier
* Memahami karakteristik dataset

Hasil analisis menunjukkan bahwa:

* Distribusi data seimbang
* Likes, comments, dan shares memiliki korelasi yang kuat
* Terdapat outlier karena adanya konten yang sangat viral

---

## 🛠️ Tech Stack

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* Seaborn
* Matplotlib

---

## 🚀 Cara Menjalankan Project

1. Buka file notebook di Google Colab
2. Upload dataset CSV
3. Jalankan seluruh cell secara berurutan
4. Lihat hasil evaluasi model

---

## 📌 Kesimpulan

Model Machine Learning yang dibangun mampu melakukan klasifikasi konten viral dengan baik dengan tingkat akurasi sekitar **90%**.

Hasil menunjukkan bahwa fitur interaksi pengguna seperti likes, comments, dan shares memiliki pengaruh yang besar terhadap viralitas suatu konten.

---

## 👤 Author

**Nama: Aisyah Syifa karima** 

Project Mata Kuliah Machine Learning — Program Studi Informatika
