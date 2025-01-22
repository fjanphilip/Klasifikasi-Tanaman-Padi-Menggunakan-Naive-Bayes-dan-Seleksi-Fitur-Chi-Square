# Klasifikasi Tanaman Padi Menggunakan Naive Bayes dan Seleksi Fitur Chi-Square

Proyek ini merupakan implementasi machine learning untuk mengklasifikasikan kualitas tanaman padi berdasarkan fitur agronomisnya. Dua pendekatan digunakan:
1. **Naive Bayes**: Menggunakan semua fitur.
2. **Naive Bayes dengan Seleksi Fitur**: Menggunakan fitur terbaik yang dipilih menggunakan metode Chi-Square.

Aplikasi ini dilengkapi dengan antarmuka berbasis **Streamlit** yang memungkinkan pengguna untuk memasukkan data, memilih metode klasifikasi, dan mendapatkan hasil prediksi.

---

## Fitur Utama
- **Preprocessing Data**: Encoding fitur kategori, scaling fitur numerik, dan balancing data menggunakan SMOTE.
- **Klasifikasi Naive Bayes**: Menggunakan pendekatan tanpa dan dengan seleksi fitur Chi-Square.
- **Antarmuka Streamlit**: Memungkinkan pengguna berinteraksi langsung dengan model.
- **Validasi Input**: Mencegah prediksi jika input belum lengkap.

---

#Teknologi yang Digunakan
- **Python 3.7+**
- **Sckit-learn**
- **Imbalanced-learn (SMOTE)**
- **Streamlit**

---

## Cara Menjalankan Proyek

1. **Clone repository** ini ke lokal Anda:
   ```bash
   git clone https://github.com/username/repository-name.git
2. **Masuk ke Direktori Proyek**
   ```bash
   cd repository-name
3. **Install Semua Dependensi**
   ```bash
   pip install -r requirements.txt
4. **Jalankan Aplikasi Streamlit**
   ```bash
   streamlit run streamlit_app.py

---

## Input Data

| Fitur         | Deskripsi               | Contoh Nilai        |
|---------------|-------------------------|---------------------|
| Varietas      | Jenis varietas padi     | Inpari 42, Siam-Siam|
| Panjang       | Panjang padi (cm)       | 9.5                 |
| Bentuk        | Bentuk gabah            | Bulat, Panjang      |
| Warna         | Warna gabah             | Putih, Merah        |
| Rasa          | Rasa nasi               | Pulen, Kurang Pulen |
| Teknik        | Teknik tanam            | Konvensional        |
| Musim         | Musim tanam             | Hujan, Kemarau      |
| Hama          | Jenis hama              | Wereng Hijau        |
| pH            | Tingkat keasaman tanah  | 6.5                 |

---

## Hasil Prediksi

- Kualitas Bagus: Model memprediksi bahwa kualitas tanaman padi baik.
- Kualitas Kurang Bagus: Model memprediksi kualitas tanaman padi tidak memenuhi standar.

---

## Struktur Direktori
```plaintext
├── data.xlsx                 # Dataset tanaman padi
├── naive_bayes_model.pkl     # Model Naive Bayes tanpa seleksi fitur
├── naive_bayes_chi2_model.pkl # Model Naive Bayes dengan seleksi fitur
├── scaler.pkl                # Scaler untuk fitur numerik
├── label_encoders.pkl        # Encoder untuk fitur kategori
├── feature_names_full.pkl    # Nama fitur tanpa seleksi
├── feature_names.pkl         # Nama fitur hasil seleksi
├── streamlit_app.py          # Aplikasi Streamlit untuk prediksi
├── ChiSquare_NaiveBayes.ipynb # Notebook pelatihan model
├── requirements.txt          # Daftar dependensi

