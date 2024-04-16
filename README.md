# 2108107010003_Pertemuan_11_ANN

Soal 1 
Berisikan tentang tugas yang di kerjakan pada artikel [kedua](https://www.megabagus.id/deep-learning-artificial-neural-networks-aplikasi) menggunakan tensorflow pada python environment.
Dataset yang digunakan adalah Data_bank_chun.csv. Bisa di akses di folder Soal1.

Informasi yang dimiliki adalah;
1. RowNumber menunjukkan ia baris ke berapa.
2. CustomerId adalah identitas unik setiap costumer.
3. Surname adalah nama belakang pelanggan.
4. CreditScore adalah skor kredit yang diberikan oleh bank. Hanya bank yang tahu cara menghitung skor ini.
5. Geography adalah negara domisili nasabah.
6. Gender adalah jenis kelamin.
7. Age adalah usia.
8. Tenure adalah berapa lama (dalam tahun) mereka sudah menjadi nasabah bank.
9. Balance adalah tabungan nasabah saat ini (atau saat terakhir sebelum keluar sebagai nasabah).
10. NumberOfProduct adalah berapa banyak produk bank yang dimiliki oleh nasabah pada saat ini (atau saat terakhir).
11. HasCrCard adalah kondisi apakah saat ini nasabah memiliki kartu kredit di bank ini (1) atau tidak (0).
12. IsActiveMember adalah kondisi apakah pelanggan saat ini aktif (1) menjadi member aktif atau tidak (0). Hanya bank yang tahu cara membuat status ini, misal apakah nasabah aktif melakukan transaksi di bulan terakhir, apakah memiliki pinjaman di bulan terakhir, dan seterusnya.
13. EstimatedSalary adalah estimasi gaji yang dibuat oleh bank. Tentu saja bank tidak tahu gaji asli dari nasabah, tapi bank sudah membuat perkiraan gaji berdasarkan pola keluar masuknya uang nasabah tersebut.
14. Exited adalah status apakah nasabah ini tetap di bank (0) atau keluar dari bank (1).

Soal 2
Berisikan tugas yang sebelumnya sudah dikerjakan sebelumnya dengan metode SVM kemudian dibuatkan dengan metode ANN
Ada dua metode ann yang dilakukan.
1. Klasifikasi
    Dataset yang digunakan untuk klasifikasi adalah data.csv yang bisa di akses didalam folder soal 2. Atau bisa diakses pada https://colab.research.google.com/corgiredirector?site=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Fuciml%2Fbreast-cancer-wisconsin-data%2Fdata
   
   Informasi Atribut dataset :
   1) Nomor ID
   2) Diagnosa (M = ganas, B = jinak) 3-32)
      Sepuluh fitur bernilai nyata dihitung untuk setiap inti sel:
      a) jari-jari (rata-rata jarak dari pusat ke titik-titik pada keliling) b) tekstur (standar deviasi nilai skala abu-abu) c) keliling d) luas e) kehalusan (variasi lokal pada panjang jari-jari) f) kekompakan (keliling^2 / luas - 1,0) g) cekungan (keparahan bagian cekung dari kontur) h) titik cekung (jumlah bagian cekung dari kontur) i) simetri j) dimensi fraktal ("perkiraan garis pantai" - 1)

Rata-rata, kesalahan standar dan "terburuk" atau terbesar (rata-rata dari tiga nilai terbesar) dari fitur-fitur ini dihitung untuk setiap gambar, sehingga menghasilkan 30 fitur. Misalnya, bidang 3 adalah Radius Rata-rata, bidang 13 adalah Radius SE, bidang 23 adalah Radius Terburuk.

Semua nilai fitur dikodekan ulang dengan empat digit signifikan.

Nilai atribut tidak ada: tidak ada

Distribusi kelas : 357 jinak, 212 ganas

2. Regresi
  Dataset ini diambil dari laman : https://www.kaggle.com/code/heeraldedhia/regression-on-diamonds-dataset-95-score/input

Studi Kasus : Prediksi Harga Berlian dengan Regresi Linear Sederhana dan Polynomial.

Dataset klasik ini berisi harga dan atribut lainnya dari hampir 54.000 berlian.

Deskripsi Kolom

price price in US dollars ($326--$18,823)
carat weight of the diamond (0.2--5.01)
cut quality of the cut (Fair, Good, Very Good, Premium, Ideal)
color diamond colour, from J (worst) to D (best)
clarity a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))
x length in mm (0--10.74)
y width in mm (0--58.9)
z depth in mm (0--31.8)
depth total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)
table width of top of diamond relative to widest point (43--95)

#Kesimpulan
Dari hasil evaluasi model yang telah dilakukan, kita dapat membuat beberapa kesimpulan:

1. **Mean Squared Error (MSE):**
   - Untuk model ANN regresi, MSE sebesar 2054677.8470757403.
   - Untuk model SVR dengan kernel linier, MSE sebesar 2567648.1981319925.
   - Untuk model SVR dengan kernel RBF, MSE sebesar 2080662.9086372997.
   - MSE yang lebih rendah menunjukkan bahwa model ANN menghasilkan prediksi yang lebih dekat dengan nilai sebenarnya dibandingkan dengan model SVR dengan kedua jenis kernel.

2. **R-squared (R^2):**
   - Untuk model ANN regresi, R^2 sebesar 0.8707491397965639.
   - Untuk model SVR dengan kernel linier, R^2 sebesar 0.8384804027645074.
   - Untuk model SVR dengan kernel RBF, R^2 sebesar 0.8691145324229308.
   - R^2 yang lebih tinggi menunjukkan bahwa model ANN lebih baik dalam menjelaskan variabilitas data target dibandingkan dengan model SVR.

Dari kedua metrik evaluasi di atas, kita dapat menyimpulkan bahwa model ANN regresi memiliki kinerja yang lebih baik daripada model SVR dengan kedua jenis kernel (linier dan RBF) dalam memprediksi harga berlian. Model ANN memberikan MSE yang lebih rendah dan R^2 yang lebih tinggi, menunjukkan bahwa model ANN lebih akurat dalam memprediksi harga berlian berdasarkan atribut-atributnya dibandingkan dengan model SVR.
