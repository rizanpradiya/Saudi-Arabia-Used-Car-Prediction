
## Ringkasan
Proyek ini menganalisis data mobil bekas di Arab Saudi untuk memprediksi harga kendaraan berdasarkan karakteristik utama, sekaligus mengidentifikasi faktor yang paling berpengaruh dalam menentukan harga jual secara objektif dan kompetitif.

## Tujuan
- Membantu penjual mobil bekas dalam menentukan harga jual yang tepat dan kompetitif menggunakan pendekatan berbasis data.
- Mengembangkan model prediksi harga mobil bekas berdasarkan karakteristik kendaraan.
- Memberikan estimasi harga yang objektif untuk mendukung keputusan penjual, pembeli, dan platform jual beli mobil bekas.

## Dataset
[Source](https://www.kaggle.com/datasets/raihanmuhith/saudi-arabia-used-car/data)

**Key Features**

| Feature        | Description                                   | dtypes   |
|---------------|-----------------------------------------------|----------|
| `Type`        | Car model or variant                          | object   |
| `Region`      | Region where the car is listed                | object   |
| `Make`        | Car manufacturer                              | object   |
| `Gear_Type`   | Transmission type                             | object   |
| `Origin`      | Car origin                                    | object   |
| `Options`     | Available features or options                 | object   |
| `Year`        | Manufacturing year                            | int64    |
| `Engine_Size` | Engine capacity                               | float64  |
| `Mileage`     | Distance traveled by the car                  | int64    |
| `Negotiable`  | Indicates whether the price is negotiable     | bool     |
| `Price`       | Selling price of the car (target variable)   | int64    |


## Kesimpulan

Berdasarkan analisis korelasi, fitur `Year` memiliki hubungan positif terhadap `Price`, yang menunjukkan bahwa mobil dengan tahun produksi lebih baru cenderung memiliki harga lebih tinggi. Selain itu, fitur `Engine_Size` juga memiliki korelasi positif, yang mengindikasikan bahwa kapasitas mesin yang lebih besar cenderung memiliki harga yang sedikit lebih mahal.

Berdasarkan hasil pemodelan, fitur `Year` dan `Engine_Size` merupakan faktor yang paling berpengaruh terhadap `Price`. Proses hyperparameter tuning yang dilakukan hanya memberikan peningkatan performa model yang sangat kecil.

## Rekomendasi

### Rekomendasi Bisnis
- Menjadikan usia kendaraan sebagai faktor utama dalam penentuan harga dan strategi penawaran karena berpengaruh signifikan terhadap harga jual.
- Memanfaatkan kapasitas mesin (`Engine_Size`) sebagai diferensiasi nilai produk, terutama pada kendaraan dengan karakteristik lain yang serupa.
- Mengelola komposisi stok kendaraan dengan menyeimbangkan mobil keluaran terbaru dan variasi spesifikasi mesin untuk memaksimalkan potensi pendapatan.

### Rekomendasi Model
- Memperbarui dan memperkaya dataset agar model dapat menangkap variasi harga mobil bekas dengan lebih baik.
- Menambahkan fitur tambahan seperti kondisi fisik kendaraan atau riwayat perawatan untuk meningkatkan akurasi prediksi.
- Mengeksplorasi pendekatan pemodelan lain atau kombinasi beberapa model guna memperoleh peningkatan performa yang lebih optimal.
