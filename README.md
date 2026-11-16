# Prediksi Gaji Menggunakan Support Vector Regression (SVR)

Proyek ini merupakan implementasi algoritma **Support Vector Regression (SVR)** untuk memprediksi besaran gaji (`Salary`) berdasarkan lama pengalaman kerja (`YearsExperience`).

## Dataset
Dataset yang digunakan adalah `Salary_Data.csv`, dengan total **30 baris data** dan **2 kolom**:
* **Atribut (Fitur):** `YearsExperience` (Lama pengalaman kerja dalam tahun.
* **Label (Target):** `Salary` (Besaran gaji).

## Alur Pengerjaan
1. **Import & Eksplorasi Data:** Membaca dataset menggunakan `pandas` serta memeriksa struktur dan tipe data dengan `.info()` dan `.head()` (seluruh data sudah lengkap dan bertipe numerik `float64`, sehingga tidak diperlukan proses *encoding*).
2. **Pemisahan & Penyesuaian Dimensi Data:** Memisahkan kolom atribut `YearsExperience` (`X`) dan label `Salary` (`y`), lalu mengubah bentuk array atribut menjadi 2 dimensi menggunakan `numpy` (`np.newaxis`) agar sesuai dengan format input model.
3. **Pelatihan Model (SVR):** Membangun dan melatih model `SVR` menggunakan `scikit-learn` dengan parameter `C=1000`, `gamma=0.05`, dan `kernel='rbf'`.
4. **Visualisasi Hasil:** Menampilkan grafik sebaran data asli menggunakan `.scatter()` dan garis kurva hasil prediksi model menggunakan `.plot()` dari library `matplotlib`.

## Teknologi & Library yang Digunakan
* **Python 3**
* **Pandas** (Manipulasi dan analisis data)
* **NumPy** (Pengolahan dimensi array)
* **Scikit-Learn** (`SVR`)
* **Matplotlib** (Visualisasi data dan garis prediksi)
