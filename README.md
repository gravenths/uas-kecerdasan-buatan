# Comparison of K-Nearest Neighbors (KNN) and Support Vector Machine (SVM) Algorithms for Bank Customer Churn Prediction

This paper discusses a performance comparison between two machine learning algorithms, K-Nearest Neighbors (KNN) and Support Vector Machine (SVM), in predicting customer churn using a bank customer dataset. Both algorithms were trained and evaluated using multiple classification metrics to determine the superior approach for handling class-imbalanced data.

## Abstract

In this study, KNN and SVM were applied to bank customer churn classification using the following approach:

1. **Data Preprocessing**
   The dataset was normalized using `StandardScaler` and categorical variables were encoded using `LabelEncoder` prior to model training.

2. **Model Training and Evaluation**
   The dataset was split at an 80:20 ratio for training and testing. Experimental results show:

   * The KNN model (k=5) achieved an accuracy of **82.20%** with a churn class precision of 0.59.
   * The SVM model (RBF kernel) achieved an accuracy of **85.45%** with a churn class precision of 0.79.
   * The SVM model proved superior in minimizing false positives (37 vs. 88 in KNN).

## Dataset

* **Name:** Churn Modelling (`UAS_Churn_Modelling.csv`)
* **Total Samples:** 10,000 customer records
* **Number of Features:** 14 columns (including the target variable `Exited`)
* **Source:** The CSV file was provided by the course lecturer and is **not a self-made dataset**.

## Libraries Used

* Python 3.x
* Google Colaboratory
* Python Libraries:
  * `pandas`
  * `numpy`
  * `scikit-learn`

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/gravenths/uas-kecerdasan-buatan.git
cd uas-kecerdasan-buatan
```

2. Upload the `UAS_Churn_Modelling.csv` file to Google Colab when prompted, or place it in the same directory if running locally.

3. Run the notebook `C030324011 Aufa - Evaluation of a Classification Model: KNN Vs SVM.ipynb` cell by cell in order.


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
