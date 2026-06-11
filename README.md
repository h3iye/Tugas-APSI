# Tugas APSI Pertemuan 9
# Studi kasus:

Analisis dan Perancangan Sistem Informasi Penjualan Online (E-Commerce)

# BRD (Business Requirements Document)
Sistem penjualan online dibutuhkan untuk mempermudah pelanggan dalam melakukan pembelian produk secara digital tanpa harus datang ke toko fisik. Sistem ini mencakup proses melihat katalog produk, pemesanan, pembayaran, hingga pengiriman barang. Dengan adanya sistem ini, admin dapat mengelola produk dan pesanan secara terpusat, status pesanan dapat dipantau secara real-time oleh pelanggan, dan seluruh transaksi tercatat dengan rapi sehingga mengurangi kesalahan pencatatan manual serta mempercepat proses bisnis penjualan.
ERD

Pelanggan → Menyimpan data pelanggan (nama, email, nomor HP, alamat).
Kategori → Data kategori produk untuk pengelompokan barang.
Produk → Menyimpan data produk yang dijual (nama produk, harga, stok).
Pesanan → Data transaksi pemesanan (tanggal pesanan, status, total harga).
Detail_Pesanan → Rincian produk yang dibeli dalam satu pesanan (jumlah, subtotal).
Pembayaran → Data pembayaran pesanan (metode pembayaran, jumlah bayar, tanggal bayar).

# Flow Bisnis

Pelanggan melihat katalog dan memilih produk, lalu menambahkannya ke keranjang.
Pelanggan melakukan checkout dan mengisi alamat pengiriman.
Sistem menghitung total belanja beserta ongkos kirim, lalu membuat pesanan dengan status "Menunggu Pembayaran".
Pelanggan melakukan pembayaran; sistem memverifikasi — jika valid, status berubah menjadi "Dibayar", jika tidak, pesanan dibatalkan.
Admin memverifikasi pesanan, menyiapkan barang, dan menginput nomor resi.
Kurir mengirim barang ke alamat pelanggan.
Pelanggan menerima barang dan melakukan konfirmasi, lalu sistem mengubah status pesanan menjadi "Selesai".


Catatan: di screenshot tugasmu studi kasusnya tentang "Analisis Hubungan Usia, Produktivitas, dan Konsumsi Gula" — itu beda tema dengan diagram penjualan yang kita buat. Kalau ternyata dosen mewajibkan pakai tema kesehatan itu, bilang saja, nanti saya buatkan ulang PlantUML flow bisnis + ERD-nya sesuai entitas Respondent, CognitiveTest, SugarConsumption, dst.
