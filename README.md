# tugasperbab-mlearning-bab4
---

## 4. Praktikum Bab 4: Feature Selection & Pipeline

### 1. Perbandingan Feature Selection:
- **SelectKBest (Filter Method):** Memilih fitur berdasarkan uji statistik univariat dengan cepat tanpa melibatkan model machine learning.
- **RFE (Wrapper Method):** Melakukan seleksi fitur secara berulang dengan melatih model dan membuang fitur yang memiliki koefisien paling kecil.
- **Lasso (Embedded Method):** Melakukan seleksi fitur secara otomatis selama proses pelatihan model melalui regularisasi L1.

### 2. Membangun Pipeline Lengkap (Dataset Titanic):
- **ColumnTransformer:** Digunakan untuk memisahkan penanganan data numerik (*imputasi median* dan *standard scaler*) dan data kategorikal (*imputasi modus* dan *one-hot encoding*).
- **Pipeline:** Menggabungkan seluruh tahapan *preprocessing* hingga model klasifikasi (`LogisticRegression`) ke dalam satu objek utuh.
- **Manfaat:** Proses *deployment* menjadi jauh lebih sederhana, terstruktur, dan meminimalisir risiko kesalahan manipulasi data pada data baru[cite: 5].
