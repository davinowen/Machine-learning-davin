📊 Supervised Learning: Linear Regression
🏡 Prediksi Harga Rumah (USA Housing Dataset)

📌 Gambaran Umum
Project ini berfokus pada pembuatan model prediksi harga rumah menggunakan pendekatan Linear Regression. Data yang digunakan berisi beberapa faktor yang secara umum memengaruhi harga rumah, seperti pendapatan rata-rata wilayah, usia rumah, jumlah ruangan, jumlah kamar tidur, serta populasi area tersebut.

Kolom alamat sengaja tidak digunakan karena tidak memberikan nilai numerik yang relevan untuk model.

📂 Data yang Digunakan
Dataset: USA_Housing.csv

Variabel yang digunakan:

Pendapatan rata-rata area
Usia rata-rata rumah
Jumlah rata-rata ruangan
Jumlah kamar tidur
Populasi area

Target yang diprediksi:

Harga rumah

⚙️ Tools & Library
Pengolahan data dan pemodelan dilakukan menggunakan Python dengan bantuan beberapa library utama seperti:
pandas dan numpy untuk manipulasi data, matplotlib dan seaborn untuk visualisasi, serta scikit-learn untuk membangun model regresi.

🔍 Alur Pengerjaan

Pertama, data dimuat dan dibersihkan dengan menghapus kolom yang tidak diperlukan. Setelah itu, data dipisahkan menjadi fitur (X) dan target (y).

Selanjutnya dilakukan eksplorasi data untuk memahami pola dan hubungan antar variabel. Ini termasuk melihat distribusi data dan korelasi antar fitur menggunakan visualisasi.

Dataset kemudian dibagi menjadi data training (70%) dan testing (30%) agar model bisa diuji pada data yang belum pernah dilihat sebelumnya.

Model Linear Regression kemudian dilatih menggunakan data training, dan menghasilkan nilai intercept serta koefisien untuk masing-masing fitur.

📈 Evaluasi Model

Performa model diukur menggunakan beberapa metrik:

MAE menunjukkan rata-rata selisih antara prediksi dan nilai aktual
RMSE memberikan gambaran error yang lebih sensitif terhadap nilai ekstrem
R² Score menunjukkan seberapa baik model menjelaskan variasi data

Hasilnya:
Model memiliki nilai R² sekitar 0.92, yang berarti model mampu menjelaskan sebagian besar variasi harga rumah dengan cukup baik.

Nilai MAE yang rendah menunjukkan bahwa secara umum prediksi cukup akurat. Namun, RMSE yang sedikit lebih tinggi mengindikasikan adanya beberapa data yang menyimpang (outlier).

📊 Insight dari Model

Dari hasil analisis:

Usia rumah dan jumlah ruangan memiliki pengaruh paling besar terhadap harga
Pendapatan area juga berperan penting dan konsisten
Jumlah kamar tidur ternyata tidak terlalu signifikan dibanding fitur lainnya

🧪 Pengujian Asumsi

Beberapa asumsi dasar regresi juga diperiksa:

Distribusi residual cenderung normal
Tidak terlihat pola khusus pada residual (cukup homoskedastis)
Masih ada beberapa outlier yang bisa memengaruhi hasil model

✅ Kesimpulan

Model Linear Regression yang dibangun sudah bekerja dengan cukup baik dalam memprediksi harga rumah. Sebagian besar pola dalam data berhasil ditangkap oleh model, meskipun masih ada pengaruh dari beberapa nilai ekstrem.

Jika ingin meningkatkan performa, langkah selanjutnya bisa fokus pada penanganan outlier atau mencoba model yang lebih kompleks.