# 🏠 Prediksi Harga Rumah Menggunakan Regresi Linier

Proyek ini merupakan implementasi sederhana dari **machine learning regresi linier** untuk memprediksi **harga rumah (dalam Rupiah)** berdasarkan **luas rumah (dalam meter persegi)**. Kode ini merupakan pengembangan dari konsep dasar *Model Representation* (Andrew Ng's Machine Learning Course), tetapi telah dimodifikasi agar sesuai dengan konteks Indonesia.

## 📘 Deskripsi Proyek

Model ini menggunakan **dua data pelatihan (training data)** untuk belajar hubungan antara luas rumah dan harganya. Tujuan utamanya adalah untuk memahami bagaimana sebuah model linier dengan fungsi:

\[
f_{w,b}(x) = w \times x + b
\]

dapat digunakan untuk melakukan prediksi harga rumah baru.

## ⚙️ Fitur Utama

- Menggunakan **NumPy** untuk perhitungan numerik
- Menggunakan **Matplotlib** untuk visualisasi hasil model
- Implementasi **manual dari gradient descent**, tanpa library machine learning tambahan
- Satuan disesuaikan dengan konteks Indonesia:
  - Luas rumah → meter persegi (m²)
  - Harga rumah → Rupiah (Rp)

## 📊 Dataset Contoh

| Luas Rumah (m²) | Harga Rumah (Rp) |
|-----------------|------------------|
| 100             | 300,000,000      |
| 200             | 500,000,000      |

Model akan belajar dari dua data ini untuk menentukan parameter **kemiringan (w)** dan **bias (b)**.

## 🧠 Algoritma yang Digunakan

1. **Model Linier**
   \[
   f_{w,b}(x) = w \times x + b
   \]

2. **Fungsi Biaya (Cost Function)**
   Menggunakan *Mean Squared Error (MSE)*:
   \[
   J(w,b) = \frac{1}{2m} \sum_{i=1}^{m}(f_{w,b}(x^{(i)}) - y^{(i)})^2
   \]

3. **Gradient Descent**
   Algoritma
