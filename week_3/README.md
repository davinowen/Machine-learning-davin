Feature Engineering untuk Persiapan Machine Learning

Project ini berfokus pada tahap awal dalam machine learning, yaitu pengolahan dan persiapan data (feature engineering) sebelum data digunakan untuk training model.

Data yang Digunakan

Dalam project ini digunakan beberapa dataset, yaitu:

California Housing
Data perusahaan (company.csv)
Telco Customer Churn
Tahapan Pengolahan Data
🔸 Penanganan Outlier

Untuk mendeteksi dan menangani nilai yang tidak wajar (outlier), digunakan metode IQR (Interquartile Range).

Beberapa kolom yang diperiksa:

MedInc
HouseAge
AveRooms
AveBedrms
AveOccup

Dari hasil analisis, penanganan outlier dilakukan pada kolom MedInc.

🔸 Mengatasi Missing Value

Pada dataset company.csv, terdapat beberapa data yang kosong.

Strategi yang digunakan:

Data numerik → diisi dengan nilai tengah (median)
Data kategorikal → diisi dengan nilai yang paling sering muncul (mode)

Contoh kasus:

Kolom Headquarters memiliki nilai kosong dan diisi menggunakan mode.
🔸 Transformasi Data Kategorikal (Encoding)

Karena model machine learning hanya bisa membaca angka, maka data kategorikal perlu diubah menjadi numerik.

Metode yang digunakan:

1. One Hot Encoding

Digunakan pada kolom: gender

2. Label Encoding

Digunakan pada beberapa kolom seperti:
Partner, Dependents, StreamingMovies, StreamingTV, TechSupport, DeviceProtection, OnlineBackup, OnlineSecurity, dan MultipleLines

3. Mean Encoding

Diterapkan pada kolom: Contract
Nilai diubah berdasarkan rata-rata target Churn
Library yang Digunakan

Beberapa library Python yang dipakai dalam project ini antara lain:

pandas
numpy
matplotlib
seaborn
scikit-learn
Pembuat

Davin Daniswara Owen Modok