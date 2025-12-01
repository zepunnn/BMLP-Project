# 📊 Customer Behavior Analytics & Prediction System

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)

## 📝 Gambaran Proyek

Repository ini berisi solusi *end-to-end* machine learning untuk menganalisis perilaku transaksi pelanggan. Proyek ini dibagi menjadi dua modul utama:
1.  **Clustering (Unsupervised Learning):** Melakukan segmentasi pelanggan untuk memahami pola belanja dan profil demografis.
2.  **Klasifikasi (Supervised Learning):** Membangun model prediktif untuk mengklasifikasikan data pelanggan baru secara otomatis.

Proyek ini dibuat sebagai bagian dari Submission Akhir BMLP.

---

## 🔍 Metodologi & Pendekatan

### 1. Customer Segmentation (Clustering)
Menggunakan algoritma **K-Means** untuk mengelompokkan pelanggan berdasarkan kemiripan fitur transaksi dan demografi.
* **Teknik:** Elbow Method & Silhouette Score untuk menentukan jumlah cluster optimal ($k=3$).
* **Preprocessing:** Scaling data, PCA (Principal Component Analysis) untuk reduksi dimensi.
* **Insight Persona:**
    * **Cluster 0 (Student - Saver):** Kelompok pelajar dengan pengeluaran terendah, berlokasi dominan di Charlotte.
    * **Cluster 1 (Student - High Spender):** Kelompok pelajar muda namun dengan nilai transaksi tertinggi (impulsif/mampu), dominan di Tucson.
    * **Cluster 2 (Professional - Engineer):** Kelompok profesional mapan dengan durasi transaksi terlama, dominan di Fort Worth.

### 2. Predictive Modeling (Klasifikasi)
Menggunakan algoritma **Random Forest Classifier** untuk memprediksi kategori pelanggan atau target variabel berdasarkan fitur yang ada.
* **Model:** Random Forest.
* **Evaluasi:** Confusion Matrix, Accuracy Score, dan Classification Report.

---

## 🛠️ Teknologi yang Digunakan

* **Bahasa:** Python
* **Data Processing:** Pandas, NumPy
* **Visualisasi:** Matplotlib, Seaborn, Yellowbrick
* **Machine Learning:** Scikit-Learn (KMeans, RandomForest)

---

## 🚀 Cara Menjalankan Project

1.  **Clone repository ini:**
    ```bash
    git clone [https://github.com/username-anda/nama-repo.git](https://github.com/username-anda/nama-repo.git)
    ```
2.  **Install library yang dibutuhkan:**
    Pastikan Anda memiliki library `yellowbrick` dan library standar lainnya.
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn yellowbrick
    ```
3.  **Buka Notebook:**
    Jalankan Jupyter Notebook atau VS Code untuk membuka file `.ipynb`.
    * `[Clustering]_Submission_Akhir...ipynb` untuk melihat analisis segmentasi.
    * `[Klasifikasi]_Submission_Akhir...ipynb` untuk melihat model prediksi.

---

## 📈 Hasil & Kesimpulan

Analisis ini berhasil memetakan karakteristik unik pelanggan yang tidak terlihat hanya dengan melihat data mentah. Meskipun rentang nilai *Amount* dan *Age* antar kelompok terlihat tipis, kombinasi dengan data kategorikal (Pekerjaan & Lokasi) memberikan separasi yang jelas untuk strategi bisnis yang lebih terarah.

---

**Author:** Fakhri Muhammad Al Hisyam
