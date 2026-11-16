# Implementasi Algoritma Support Vector Machine (SVM)

Repositori ini dibuat untuk menyelesaikan tugas dan praktikum mengenai penerapan algoritma **Support Vector Machine (SVM)**, baik untuk kasus klasifikasi (*Support Vector Classification*) maupun regresi (*Support Vector Regression*) menggunakan pustaka `scikit-learn` di Python.

---

## 📂 Struktur Berkas & Notebook

1. **`svm.ipynb` (Klasifikasi Linear & Margin)**
   * **Deskripsi:** Membangun model `SVC` dengan kernel linear (`kernel='linear'`) untuk memprediksi kelulusan ujian berdasarkan jam belajar dan jam tidur[cite: 1].
   * **Fitur:** Visualisasi *decision boundary* (hyperplane) beserta margin positif dan negatif menggunakan `matplotlib`[cite: 1].

2. **`salary data.ipynb` (Support Vector Regression / SVR)**
   * **Deskripsi:** Menerapkan model `SVR` dengan kernel RBF (`kernel='rbf'`), parameter regularisasi $C=1000$, dan $\gamma=0.05$[cite: 2].
   * **Fitur:** Membaca dataset dari file CSV (`Salary_Data.csv`) untuk melakukan prediksi gaji berdasarkan lama pengalaman kerja (*Years of Experience*)[cite: 2].

3. **`diabetes.ipynb` (Klasifikasi Medis / SVC)**
   * **Deskripsi:** Menerapkan klasifikasi biner menggunakan `SVC` pada dataset diabetes (`diabetes.csv`) yang memiliki 8 fitur medis (seperti kadar glukosa, BMI, tekanan darah, dll.)[cite: 3].
   * **Fitur:** 
     * Pra-pemrosesan data menggunakan standarisasi (`StandardScaler`)[cite: 3].
     * Pembagian data latih dan uji dengan fungsi `train_test_split`[cite: 3].
     * Evaluasi tingkat akurasi model pada data uji[cite: 3].

---

## 🛠️ Kebutuhan Sistem (Dependencies)

Sebelum menjalankan kode di dalam notebook, pastikan pustaka berikut sudah terinstal di lingkungan Python Anda:

```bash
pip install numpy pandas matplotlib scikit-learn
