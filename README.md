# Perbandingan Algoritma K-Nearest Neighbors (KNN) dan Support Vector Machine (SVM) untuk Prediksi Churn Pelanggan Bank

Makalah ini membahas perbandingan performa dua algoritma *machine learning*, yaitu K-Nearest Neighbors (KNN) dan Support Vector Machine (SVM), dalam memprediksi *customer churn* pada dataset nasabah bank. Kedua algoritma diuji dan dievaluasi menggunakan berbagai metrik klasifikasi untuk menentukan pendekatan yang lebih unggul dalam menangani data dengan distribusi kelas yang tidak seimbang.

## Abstrak

Dalam penelitian ini, KNN dan SVM diterapkan untuk klasifikasi *churn* pelanggan bank menggunakan pendekatan berikut:

1. **Preprocessing Data**
   Dataset dinormalisasi menggunakan `StandardScaler` dan variabel kategorikal di-*encode* menggunakan `LabelEncoder` sebelum pelatihan model.

2. **Pelatihan dan Evaluasi Model**
   Dataset dibagi dengan rasio 80:20 untuk data latih dan data uji. Hasil percobaan menunjukkan:

   * Akurasi model KNN (k=5) mencapai **82,20%** dengan *precision* kelas *churn* sebesar 0,59.
   * Akurasi model SVM (kernel RBF) mencapai **85,45%** dengan *precision* kelas *churn* sebesar 0,79.
   * Model SVM terbukti lebih unggul dalam meminimalkan *false positive* (37 vs. 88 pada KNN).

## Dataset

* **Nama:** Churn Modelling (`UAS_Churn_Modelling.csv`)
* **Jumlah Sampel:** 10.000 data nasabah
* **Jumlah Fitur:** 14 kolom (termasuk variabel target `Exited`)
* **Sumber:** File CSV diperoleh dari dosen pengampu mata kuliah dan **bukan merupakan dataset buatan sendiri**.

## Pustaka yang Digunakan

* Python 3.x
* Google Colaboratory
* Pustaka Python:
  * `pandas`
  * `numpy`
  * `scikit-learn`

## Cara Menjalankan Kode

1. *Clone* repository ini:

```bash
git clone https://github.com/gravenths/uas-kecerdasan-buatan.git
cd uas-kecerdasan-buatan
```

2. Unggah file `UAS_Churn_Modelling.csv` ke Google Colab saat diminta, atau letakkan di direktori yang sama jika dijalankan secara lokal.

3. Jalankan notebook `C030324011 Aufa - Evaluation of a Classification Model: KNN Vs SVM.ipynb` sel per sel secara berurutan.
