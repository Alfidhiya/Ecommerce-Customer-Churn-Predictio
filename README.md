# Ecommerce-Customer-Churn-Prediction
Repositori ini berisi proyek machine learning untuk memprediksi kemungkinan customer churn pada sebuah platform e-commerce menggunakan algoritma klasifikasi. Tujuan dari proyek ini adalah membantu perusahaan dalam mengidentifikasi pelanggan yang kemungkinan besar akan berhenti menggunakan layanan.

## Tujuan
- Membangun model *machine learnin* yang dapat memprediksi pelanggan yang akan *churn* dan pelanggan *not churn*.
- Membangun model *machine learning* yang dapat diinterpretasikan sehingga mampu mengetahui faktor-faktor yang menyebabkan *churn*.
- Mendukung strategi retensi pelanggan yang tepat dan efisien.

## Teknologi yang Digunakan
- Bahasa Pemrograman
  + Python — Bahasa pemrograman utama untuk pemrosesan data dan machine learning.
- Library & Framework
  + Pandas — Untuk manipulasi dan analisis data.
  + NumPy — Untuk perhitungan numerik dan operasi array.
  + Matplotlib & Seaborn — Untuk visualisasi data.
  + Scikit-learn — Untuk preprocessing data, pembagian data, pelatihan model, dan evaluasi.
  + XGBoost — Untuk implementasi model Gradient Boosted Decision Trees.
- Environment
  + Jupyter Notebook — Untuk eksplorasi data interaktif dan dokumentasi langkah-langkah proyek.

## Struktur Proyek
├── README.md                                    <- Penjelasan singkat terkait proyek yang dibuat.
├── Data
│   ├── data_ecommerce_customer_churn.csv        <- Dataset
│   ├── Ecommerce Customer Churn.pdf             <- Penjelasan dataset
|
├── Model
│   ├── model_XGBoost_Ecommerce_Churn.sav        <- Model Pickle
│   ├── model_XGBoost_Ecommerce_Churn_joblib     <- Model Joblib
│
├── Notebook
│   ├── Ecommerce Customer Churn Prediction.ipynb  <- Jupyter Notebook dari Proyek yang dibuat
│
└── requirements.txt                               <- Requirements yang dibutuhkan

## Kesimpulan
**Model --> Extreme Gradient Boosting (XGBoost)**

**Apa itu XGBoost?**

XGBoost (Extreme Gradient Boosting) Model adalah algoritma machine learning berbasis pohon keputusan (decision tree) yang menggunakan teknik boosting untuk meningkatkan akurasi model prediktif.

**Bagaimana cara kerja XGBoost?**
- Boosting --> Membuat model secara berurutan dimana model selanjutnya memperbaiki kesalahan model sebelumnya.
- Gradient Descent --> Kesalahan model dihitung dan digunakan untuk memperbaiki model berikutnya melalui pendekatan gradien.
- Kemudian semua model kecil digabung membentuk final model yang kuat.

**Spesifikasi Model**
- n_estimators = 200
- max_depth = 11
- learning_rate = 0.2

**Train Set F2 Score:**
- Before tuning: 0.77
- After tuning: 0.78

**Test Set F2 Score:**
-  Before tuning: 0.85
-  After tuning: 0.86

Metric F2 Score digunakan karena cost function dari False Negative dianggap hampir sama besar dengan cost False Positif namun lebih memperhatikan false negatif karena lebih tinggi costnya, sehingga jumlah FN maupun FP harus balance (sama-sama rendah) dengan FN lebih rendah. 

## Kontak
- Name : Alfidhiya Amany R.
- Email : alfidhiya12@gmail.com
- LinkedIn : [LinkedIn Alfi](https://www.linkedin.com/in/alfidhiya-amany-ramli-22b79228a/)
