# Tugas APSI Pertemuan 9
Studi kasus:

Perancangan Sistem Informasi Penjualan Online (E-Commerce) untuk Mendukung Proses Transaksi, Pengelolaan Produk, dan Pengiriman Barang

# BRD (Business Requirements Document)
1. Latar Belakang
Perkembangan teknologi informasi mendorong pelaku usaha untuk beralih dari penjualan konvensional ke penjualan berbasis online. Proses penjualan yang masih dilakukan secara manual menimbulkan berbagai kendala, seperti pencatatan pesanan yang tidak terorganisir, kesulitan memantau stok produk, proses pembayaran yang tidak terverifikasi dengan baik, serta tidak adanya pelacakan status pengiriman. Oleh karena itu, dibutuhkan sebuah sistem informasi penjualan online yang mampu mengelola seluruh proses bisnis secara terintegrasi, mulai dari pemilihan produk oleh pelanggan hingga barang diterima.
2. Tujuan Bisnis

Mempermudah pelanggan dalam melihat katalog, memesan, dan membayar produk secara online.
Membantu admin dalam mengelola data produk, stok, dan verifikasi pesanan secara efisien.
Menyediakan pencatatan transaksi yang akurat dan terdokumentasi untuk kebutuhan laporan penjualan.
Memberikan transparansi status pesanan (menunggu pembayaran, dibayar, dikirim, selesai) kepada pelanggan.

3. Ruang Lingkup Sistem
Sistem mencakup pengelolaan data pelanggan, katalog produk dan kategori, keranjang belanja, pemesanan, pembayaran, hingga pencatatan pengiriman dengan nomor resi. Sistem tidak mencakup integrasi langsung dengan pihak ekspedisi (input resi dilakukan manual oleh admin).
4. Pemangku Kepentingan (Stakeholders)

Pelanggan → Pengguna yang melakukan pencarian produk, pemesanan, pembayaran, dan konfirmasi penerimaan barang.
Admin → Pengelola sistem yang memverifikasi pesanan, mengelola produk dan stok, serta menginput nomor resi.
Kurir → Pihak yang melakukan pengiriman barang kepada pelanggan.
Pemilik Usaha → Pihak yang memanfaatkan laporan penjualan untuk pengambilan keputusan bisnis.

5. Kebutuhan Fungsional

Sistem dapat menampilkan katalog produk berdasarkan kategori.
Sistem dapat mengelola keranjang belanja dan proses checkout.
Sistem dapat menghitung total harga beserta ongkos kirim secara otomatis.
Sistem dapat mencatat dan memverifikasi pembayaran pelanggan.
Sistem dapat memperbarui status pesanan di setiap tahapan transaksi.
Sistem dapat mencatat nomor resi pengiriman dan menampilkannya kepada pelanggan.

# ERD

Pelanggan → Menyimpan data pelanggan (nama, email, nomor HP, alamat) sebagai pihak yang melakukan transaksi pemesanan.
Kategori → Data pengelompokan produk (misalnya pakaian, elektronik, aksesori) untuk memudahkan pencarian.
Produk → Menyimpan data barang yang dijual (nama produk, harga, stok) dan terhubung dengan kategori.
Pesanan → Mencatat transaksi pemesanan pelanggan beserta tanggal, status pesanan, dan total harga.
Detail_Pesanan → Merinci produk apa saja yang dibeli dalam satu pesanan beserta jumlah dan subtotalnya (tabel penghubung antara Pesanan dan Produk).
Pembayaran → Menyimpan data pembayaran pesanan (metode pembayaran, jumlah bayar, tanggal bayar) sebagai bukti transaksi.


Penjelasan relasinya kalau ditanya dosen: satu Kategori memiliki banyak Produk; satu Pelanggan dapat membuat banyak Pesanan; satu Pesanan terdiri dari satu atau lebih Detail_Pesanan; satu Produk bisa muncul di banyak Detail_Pesanan; dan satu Pesanan dibayar dengan tepat satu Pembayaran.
