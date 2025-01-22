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
