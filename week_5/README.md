📊 Supervised Learning – Klasifikasi (Iris Dataset)

🌸 Klasifikasi Spesies Bunga dengan KNN

📌 Gambaran Project
Project ini dibuat untuk mengklasifikasikan spesies bunga Iris menggunakan algoritma K-Nearest Neighbors (KNN). Model akan mengenali jenis bunga berdasarkan ukuran sepal dan petal yang dimiliki setiap sampel.

Dataset yang digunakan adalah Iris Dataset, yang cukup populer dalam machine learning karena strukturnya sederhana tapi efektif untuk latihan klasifikasi.

📂 Dataset
File yang digunakan: iris.csv

Isi dataset:

150 data sampel
4 fitur numerik

Fitur yang digunakan meliputi:

Panjang sepal
Lebar sepal
Panjang petal
Lebar petal

Target yang diprediksi adalah spesies bunga, yaitu:

Setosa
Versicolor
Virginica

⚙️ Tools & Library
Seluruh proses dikerjakan menggunakan Python dengan bantuan:
pandas dan numpy untuk pengolahan data, matplotlib dan seaborn untuk visualisasi, serta scikit-learn untuk pemodelan dan evaluasi.

🔍 Alur Pengerjaan

Data pertama kali dimuat menggunakan pandas, kemudian dilanjutkan dengan eksplorasi untuk memahami karakteristik dataset. Pada tahap ini dilakukan pengecekan struktur data, statistik dasar, serta visualisasi seperti distribusi fitur dan perbandingan antar kelas.

Setelah itu, data dipersiapkan dengan mengecek missing value dan mengubah label kategori menjadi numerik menggunakan LabelEncoder. Dataset kemudian dibagi menjadi data training (70%) dan testing (30%).

Karena KNN sangat bergantung pada jarak, fitur dinormalisasi menggunakan StandardScaler agar semua variabel berada pada skala yang sama.

Model KNN kemudian dilatih menggunakan data training. Selain menggunakan parameter default, dilakukan juga tuning untuk mencari kombinasi parameter terbaik.

🛠️ Hyperparameter Tuning

Untuk mendapatkan hasil optimal, dilakukan pencarian parameter terbaik menggunakan GridSearchCV dengan beberapa kombinasi:

jumlah tetangga (n_neighbors)
metode pembobotan (weights)
jenis perhitungan jarak (metric)

Evaluasi dilakukan menggunakan metrik seperti accuracy, precision, recall, dan F1-score.

📈 Hasil & Analisis

Model KNN menunjukkan performa yang sangat baik dengan tingkat akurasi yang tinggi, bahkan bisa mendekati 100% tergantung parameter yang digunakan.

Hasil terbaik diperoleh setelah proses tuning, yang membantu model memilih jumlah tetangga dan metode jarak yang paling sesuai dengan pola data.

🔮 Penggunaan Model

Model yang sudah dilatih bisa digunakan untuk memprediksi data baru. Misalnya, dengan memasukkan ukuran sepal dan petal tertentu, model akan mengembalikan prediksi spesies bunga tersebut.

📁 Output

Hasil dari proses tuning disimpan dalam file Excel untuk analisis lebih lanjut:
hasil_gridsearch_knn.xlsx