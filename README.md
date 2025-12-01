#  Project: Prediksi Kelulusan Mahasiswa Menggunakan SVM

Repository ini berisi implementasi lengkap Machine Learning menggunakan
**Support Vector Machine (SVM)** untuk memprediksi status kelulusan
mahasiswa berdasarkan berbagai fitur akademik.

------------------------------------------------------------------------

## 1.  Deskripsi Singkat

Proyek ini dilakukan sebagai tugas Machine Learning dengan studi kasus:

**"Prediksi Kelulusan Mahasiswa menggunakan Support Vector Machine
(SVM)"**

Model membagi mahasiswa menjadi dua kategori: - **Lulus** - **Tidak
Lulus**

Teknik yang digunakan: - Exploratory Data Analysis (EDA) - Preprocessing
(Encoding, Scaling) - Algoritma SVM (Linear & RBF) - Hyperparameter
Tuning - Evaluasi Model - Deployment fungsi prediksi sederhana

------------------------------------------------------------------------

## 2.  Dataset

Nama file: **datakelulusanmahasiswa.csv**

Contoh fitur yang digunakan: - IPK\
- Total SKS\
- Umur\
- Lama Studi\
- Kehadiran\
- Nilai Mata Kuliah\
- Label: **Status_Lulus**

Dataset dimuat menggunakan Pandas.

------------------------------------------------------------------------

## 3.  Langkah Pengerjaan (Sesuai Instruksi Tugas)

A. Setup & Loading Dataset

-   Import library
-   Load data
-   Cek info & missing values

B. Exploratory Data Analysis

Visualisasi: - Histogram IPK\
- Countplot kelulusan\
- Boxplot IPK vs Kelulusan

Menjawab pertanyaan analitis: - Apakah IPK memengaruhi kelulusan? -
Fitur mana yang paling berpengaruh?

C. Preprocessing

-   Menghapus missing value
-   Label Encoding untuk kategori
-   StandardScaler → **wajib** untuk SVM
-   Train-test split (80:20)

D. Training Model

Model dilatih: - SVM Linear\
- SVM RBF

Evaluasi: - Accuracy - Precision, Recall, F1-score - Confusion matrix

Tuning parameter: - C = {0.1, 1, 10} - gamma = {scale, 0.1, 1}

E. Interpretasi Model

-   Fitur paling berpengaruh
-   Penjelasan apakah data linearly separable
-   Analisis performa model

F. Deployment

Fungsi:

    predict_status(ipk, sks, umur, lamastudi)

------------------------------------------------------------------------

## 4.  Struktur Repository

     SVM-Kelulusan
    │
    ├── data/
    │   └── datakelulusanmahasiswa.csv
    │
    ├── SVM_kelulusan.ipynb
    ├── README.md
    └── screenshot/
        └── hasil_prediksi.png

------------------------------------------------------------------------

## 5.  Hasil Evaluasi Model

Isi dengan hasil model kamu, contoh:

-   **Model Terbaik:** SVM RBF\
-   **Akurasi:** 0.89\
-   **Kesimpulan:**\
    Model RBF menghasilkan decision boundary yang lebih baik dibanding
    model linear.

------------------------------------------------------------------------
## 6. 👤 Identitas Mahasiswa

-   **Nama**: (AL'ANJERI)
-   **NPM**: (2457201002382)
-   **Mata Kuliah**: Machine Learning
