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


## Struktur Folder
- `Proyek_Analisis_fruit_sales_data.ipynb`: berisi file google collab (normalisasi, process, dan visualization)
- `chart`: berisi file `.png` hasil visualisasi
- `dataset/`: berisi file CSV
- `README.md`: dokumentasi proyek
- `laporan.pdf`: laporan akhir
