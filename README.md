# Analisis Penjualan Buah di Cabang Jogja dan Seluruh Cabang

## Anggota Kelompok
- Muhammad Khoirul Yahya 
- Piter Rafflesia P
- Rachmat Dwi Agustyan
- Salma Kamila
- Vidky Adhi Pradana
- Yesa Nurul Fadillah

## Tujuan Proyek
Proyek ini bertujuan untuk menganalisis data penjualan buah dari seluruh cabang dan cabang Jogja. Analisis ini difokuskan pada:
- Mengidentifikasi buah dengan tingkat pembelian tertinggi.
- Membandingkan total penjualan antara semua cabang dan cabang Jogja.
- Menganalisis pola pembelian berdasarkan jenis buah.

## Dataset
- `Fruit Sales Data.csv`: Data penjualan dari seluruh cabang.
- `Fruit Sales Data Branch Jogja.csv`: Data penjualan dari cabang Jogja.
  
Kolom pada dataset:
- `Fruit_Name`: Nama buah
- `Weight_in_Kg`: Berat buah (Kg)
- `Total_Cost`: Total biaya
- `Purchased`: Status pembelian (Yes/No)

## Tools & Library
- Platform: Google Colab
- Bahasa: Python 3.x (default di Colab)
- Library:
  - Pandas
  - Matplotlib
  - seaborn
  - sklearn

## Proses Pemodelan Data
1. Eksplorasi awal dan pembersihan data (menghapus nilai kosong)
2. Pengelompokan data berdasarkan `Fruit_Name` dan `Purchased`
3. Perhitungan total berat dan biaya
4. Visualisasi:
   - Bar chart total penjualan per buah
   - Pie chart proporsi pembelian
   - Pie chart proporsi total cost per jenis buah
   - Bonus Grafik Scatter Plot untuk menunjukkan hubungan antara dua variabel numerik: "Weight_in_Kg" dan "Total"

## Hasil Visualisasi
Visualisasi menggambarkan buah-buah dengan penjualan tertinggi dan pola pembelian berdasarkan data seluruh cabang dan cabang Jogja.

> Gambar visualisasi akan ditampilkan di notebook atau laporan PDF.
![Preview](https://github.com/Codeventure-team6/Proyek-codeventure/blob/e0917a10b433537f8c768024f39ef969bdf5fd44/chart/Bar%20Chart%20-%20Total%20Pendapatan%20per%20Jenis%20Buah.png)

![Preview](https://github.com/Codeventure-team6/Proyek-codeventure/blob/e0917a10b433537f8c768024f39ef969bdf5fd44/chart/Pie%20Chart%20-%20Persentase%20Pendapatan%20Buah.png)

![Preview](https://github.com/Codeventure-team6/Proyek-codeventure/blob/e0917a10b433537f8c768024f39ef969bdf5fd44/chart/Pie%20Chart%20-%20Proposisi%20Pembelian.png)

![Preview](https://github.com/Codeventure-team6/Proyek-codeventure/blob/e0917a10b433537f8c768024f39ef969bdf5fd44/chart/Scatter_Plot_Berat_VS_Total_Regresi_Linear.png.png)

## Hasil dan Temuan

Visualisasi data penjualan buah dari seluruh cabang dan cabang Jogja telah menghasilkan beberapa temuan kunci:

### 1. Dominasi Penjualan Buah Tertentu

* Dari **Bar Chart Total Pendapatan per Jenis Buah**, terlihat jelas bahwa **Mangga** dan **Apel** adalah buah-buah dengan kontribusi pendapatan tertinggi di antara seluruh cabang. Hal ini menunjukkan popularitas dan permintaan pasar yang kuat untuk kedua jenis buah ini.
* **Pie Chart Persentase Pendapatan Buah** lebih lanjut menegaskan bahwa Mangga dan Apel menyumbang porsi terbesar dari total pendapatan penjualan buah. Buah lain seperti Anggur dan Pisang memiliki kontribusi yang relatif kecil.

### 2. Efisiensi Transaksi Pembelian

* **Pie Chart Proporsi Pembelian** menunjukkan bahwa mayoritas transaksi berhasil diselesaikan sebagai pembelian (`Purchased = Yes`). Ini mengindikasikan proses transaksi yang relatif efisien.
* Namun, adanya proporsi `Purchased = No` (meskipun minoritas) menandakan ada sejumlah transaksi yang tidak berakhir dengan pembelian. Ini bisa menjadi area untuk investigasi lebih lanjut guna mengidentifikasi potensi kehilangan penjualan.

### 3. Hubungan Berat dan Biaya Total

* **Scatter Plot Hubungan Berat (Kg) VS Total Biaya (Regresi Linear)** memperlihatkan adanya **hubungan positif yang kuat**: semakin berat buah yang dibeli, cenderung semakin tinggi total biayanya. Garis regresi linear memvisualisasikan tren ini.
* Penting untuk dicatat adanya **beberapa pencilan (outliers)**. Misalnya, ada satu pembelian dengan berat sedang namun biaya total sangat tinggi, dan sebaliknya, satu pembelian dengan berat tinggi namun biaya total relatif rendah. Pencilan ini mungkin memerlukan penyelidikan lebih lanjut untuk memahami anomali dalam penetapan harga atau jenis transaksi.

---

## Kesimpulan

Proyek analisis penjualan buah ini berhasil mengidentifikasi pola-pola penting dalam data penjualan. **Mangga dan Apel** secara konsisten menjadi pemimpin dalam hal pendapatan, menunjukkan prioritas dalam manajemen stok dan strategi pemasaran. Sementara mayoritas transaksi berhasil menjadi pembelian, adanya pembatalan (`Purchased = No`) membuka peluang untuk perbaikan proses. Hubungan antara berat dan biaya total sebagian besar konsisten, namun keberadaan pencilan menyoroti pentingnya pemeriksaan data lebih lanjut untuk kasus-kasus anomali.

Analisis ini memberikan wawasan berharga bagi pemilik data untuk membuat keputusan strategis terkait manajemen inventaris, strategi promosi, dan optimalisasi proses penjualan di seluruh cabang, termasuk cabang Jogja.

---

## Struktur Folder
- `Proyek_Analisis_fruit_sales_data.ipynb`: berisi file google collab (normalisasi, process, dan visualization)
- `chart`: berisi file `.png` hasil visualisasi
- `dataset/`: berisi file CSV
- `README.md`: dokumentasi proyek
- `laporan.pdf`: laporan akhir
