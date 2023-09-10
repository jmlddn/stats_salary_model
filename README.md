# stats_salary_model

Pengantar dan Latar Belakang

Terdapat sebuah dataset yang menunjukkan gaji yang dimiliki seseorang berdasarkan usia, jenis kelamin, tingkat pendidikan,   jabatan, ras, asal negara dan lama pengalaman kerja. Dari dataset tersebut, penulis ingin mengetahui pengaruh dari faktor-   faktor tersebut terhadap gaji dan melakukan prediksi gaji seseorang.
Menguji pengaruh jenis kelamin terhadap gaji dengan uji statistik.
Memprediksi gaji dari lama pengalaman kerja seseorang dengan model regresi.
Memprediksi gaji dari variabel prediktor usia, jenis kelamin, tingkat pendidikan, ras, asal negara dan lama pengalaman       kerja dengan model regresi.

Dataset

Dataset yang digunakan diambil dari kaggle.com. Dataset berisikan 6704 baris data usia, jenis kelamin, tingkat pendidikan, jabatan, lama pengalaman kerja, ras, asal negara dan besar gaji.
Sebelum diolah lebih lanjut, dilakukan persiapan dengan menghapus missing value dan duplicated data sehingga didapatkan 6704 baris data yang bisa digunakan.

Uji Statistik

Penulis ingin mengetahui pengaruh jenis kelamin terhadap besarnya gaji seseorang. Dalam dataset terdapat 2 jenis kelamin yaitu male (laki-laki (a)) dan female (perempuan (b)). Penulis akan menguji apakah rata-rata gaji laki-laki lebih besar dari rata-rata gaji perempuan.

Pemodelan Regresi

Single Predictor
Dilakukan pemodelan regresi untuk memprediksi gaji seseorang dari lama pengalaman kerjanya.

Single Predictor with Log Transformation
Dilakukan pemodelan regresi untuk memprediksi gaji seseorang dari lama pengalaman kerjanya namun dilakukan transformasi logaritmik pada variabel prediktor.

Multiple Predictors with One Interaction
Dalam pemodelan ini, digunakan semua variabel prediktor yaitu usia, jenis kelamin, tingkat pendidikan, dan lama pengalaman kerja. Ditambahkan juga satu interaksi antar variabel prediktor yaitu usia dan lama pengalaman kerja. Untuk variabel tingkat pendidikan (Education Level) diperlakukan sebagai variabel kategorikal.

Kesimpulan dan Saran

Dapat disimpulkan bahwa usia, jenis kelamin, lama pengalaman kerja, dan tingkat pendidikan, asal negara dan ras berpengaruh terhadap besaran gaji seseorang sehingga bisa digunakan untuk memprediksi besaran gaji tersebut.
Model regresi yang dibangun dengan single predictor yaitu lama pengalaman kerja menghasilkan performa yang cukup bagus dengan R-squared 0,65. Transformasi logaritmik pada model ini menghasilkan model yang lebih baik karena memiliki skor R-squared lebih tinggi yaitu 0,71.
Model regresi yang dibangun dengan semua predictor disertai interaksi antara usia dan lama pengalaman kerja, menghasilkan performa yang lebih baik dengan R-squared 0,75. Model tersebut juga menghasilkan interpretasi yang baik dengan dilakukannya centering pada variabel usia (age).
Untuk pengembangan selanjutnya dapat dilakukan percobaan untuk berbagai variasi jumlah predictor yang digunakan. Dapat juga dilakukan pengelompokan data gaji berdasarkan job tittle-nya sehingga didapatkan model regresi yang akurat untuk masing-masing jenis pekerjaan.

Referensi

Statistics for Business : Decision Making and Analysis - Robert Stine and Dean Foster
Regression and Other Stories. - Andrew Gelman, Jennifer Hill, and Aki Vehtari
The Effect: An Introduction to Research Design and Causality. Chapter 13 Huntington-Klein, N. 2021
Stats: Salary Prediction Using Regression Model https://kristalinaks.medium.com/stats-salary-prediction-using-regression-model-f5e53c254ac6
