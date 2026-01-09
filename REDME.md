# 🎯 Klasifikasi Sentimen Komentar YouTube dengan FastText

<p align="center">
  <b>Analisis Opini Digital Menggunakan Natural Language Processing (NLP)</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/NLP-Sentiment%20Analysis-blue" />
  <img src="https://img.shields.io/badge/Algorithm-FastText-green" />
  <img src="https://img.shields.io/badge/Classes-Positive%20%7C%20Neutral%20%7C%20Negative-orange" />
  <img src="https://img.shields.io/badge/Status-Completed-success" />
</p>

---

## 📌 Deskripsi Proyek

Proyek ini bertujuan untuk membangun **sistem klasifikasi sentimen komentar YouTube** menggunakan algoritma **FastText** guna menganalisis opini publik di platform digital. Sistem ini mampu mengklasifikasikan komentar ke dalam tiga kategori sentimen:

* 😊 **Positive**
* 😐 **Neutral**
* 😠 **Negative**

FastText dipilih karena efisiensi komputasinya yang tinggi serta kemampuannya dalam menangani **teks informal, typo, dan variasi ejaan** yang umum ditemukan pada komentar media sosial.

---

## 🎓 Informasi Akademik

* **Judul**: Klasifikasi Sentimen Komentar YouTube Menggunakan Algoritma FastText untuk Analisis Opini Digital
* **Nama**: Maylani Kusuma Wardhani
* **NIM**: 202210370311123
* **Program Studi**: Informatika
* **Fakultas**: Teknik
* **Universitas**: Universitas Muhammadiyah Malang
* **Tahun**: 2025

---

## 🧠 Metodologi Penelitian

Penelitian ini menggunakan pendekatan **kuantitatif eksperimental** dengan pipeline NLP terstruktur sebagai berikut:

1. **Data Collection** – Pengumpulan komentar YouTube berlabel sentimen
2. **Preprocessing Teks** – Pembersihan dan normalisasi data
3. **Feature Extraction** – Representasi teks berbasis subword (FastText)
4. **Model Training** – Supervised FastText
5. **Hyperparameter Tuning** – Grid Search
6. **Evaluation** – Accuracy, Precision, Recall, F1-Score

---

## 📂 Dataset

* **Total Data**: 18.408 komentar YouTube
* **Distribusi Kelas**:

  * Positive: 11.432 (62.1%)
  * Neutral: 4.638 (25.2%)
  * Negative: 2.338 (12.7%)

📌 Dataset bersifat **imbalanced**, mencerminkan kondisi data nyata pada media sosial.

---

## ⚙️ Preprocessing NLP

Tahapan preprocessing yang diterapkan:

* Case folding (lowercase)
* Penghapusan URL & mention
* Normalisasi teks informal
* Penanganan emoji & tanda baca penting (!!!, ???)
* Tokenisasi teks
* Selektif stopword removal

Pendekatan ini menjaga **informasi sentimen** tetap utuh tanpa menghilangkan konteks penting.

---

## 🚀 Model FastText

Konfigurasi model optimal:

| Parameter        | Nilai |
| ---------------- | ----- |
| Epoch            | 30    |
| Learning Rate    | 0.1   |
| Word N-grams     | 2     |
| Vector Dimension | 100   |

Keunggulan FastText:

* Subword information (robust terhadap typo)
* Training & inference sangat cepat
* Cocok untuk data media sosial

---

## 📊 Hasil Evaluasi

### 🔹 Performa Model

* **Accuracy**: 75.68%
* **Macro F1-Score**: 0.65
* **Weighted F1-Score**: 0.75

### 🔹 Performa per Kelas

| Sentimen | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| Positive | 0.84      | 0.89   | 0.86     |
| Neutral  | 0.60      | 0.60   | 0.60     |
| Negative | 0.52      | 0.43   | 0.49     |

📌 Model menunjukkan performa terbaik pada kelas **positive** dan tantangan pada kelas **negative** akibat ketidakseimbangan data.

---

## ⚡ Efisiensi Komputasi

* ⏱️ Training Time: ±18 detik
* 📦 Model Size: ±23 MB
* 🚀 Inference Time: < 1 ms / komentar
* 🔁 Throughput: ±2500 prediksi/detik

Sangat cocok untuk **real-time sentiment analysis**.

---

## 📈 Analisis & Insight

* Bigram efektif menangkap frasa sentimen seperti *"not good"*, *"very amazing"*
* FastText robust terhadap bahasa informal & typo
* Confusion terbesar terjadi antara **neutral ↔ positive**
* Sarkasme masih menjadi tantangan utama

---

## 🧩 Keterbatasan

* Dataset hanya mencakup satu bahasa
* Belum menangani sarkasme secara eksplisit
* Analisis masih bersifat document-level
* Tidak mempertimbangkan konteks thread komentar

---

## 🔮 Pengembangan Selanjutnya

* Multilingual & code-mixed sentiment analysis
* Ensemble & deep learning models
* Aspect-based sentiment analysis
* Multimodal sentiment (teks + video)

---

## 📌 Kesimpulan

FastText terbukti sebagai solusi **efisien, ringan, dan cukup akurat** untuk klasifikasi sentimen komentar YouTube. Dengan pipeline NLP yang tepat, model ini mampu memberikan insight opini publik secara cepat dan praktis untuk kebutuhan akademik maupun industri.

---

✨ *Dikembangkan sebagai bagian dari Tugas Besar / Project Akademik*
📍 *Informatika – Universitas Muhammadiyah Malang*
