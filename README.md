# Tugas APSI Pertemuan 9

## Studi Kasus:

Perancangan Sistem Informasi Administrasi PAUD untuk Mendukung Proses Pendaftaran, Pembayaran, dan Pengelolaan Data Siswa

# BRD (Business Requirements Document)

## 1. Latar Belakang

Pengelolaan administrasi pada PAUD umumnya masih dilakukan secara manual menggunakan buku pencatatan atau spreadsheet sederhana. Proses pendaftaran siswa, pencatatan data orang tua, pembayaran biaya pendaftaran dan SPP, serta pembuatan laporan sering kali memerlukan waktu yang lama dan berisiko terjadi kesalahan pencatatan. Selain itu, pencarian data siswa dan riwayat pembayaran menjadi kurang efisien. Oleh karena itu, diperlukan sebuah Sistem Informasi Administrasi PAUD yang mampu mengelola seluruh data siswa dan transaksi pembayaran secara terintegrasi sehingga proses administrasi menjadi lebih efektif, akurat, dan terdokumentasi dengan baik.

## 2. Tujuan Bisnis

* Mempermudah proses pendaftaran siswa baru secara terstruktur.
* Membantu pihak administrasi dalam mengelola data siswa dan orang tua.
* Mempermudah pencatatan pembayaran biaya pendaftaran dan SPP.
* Menyediakan laporan pembayaran dan data siswa secara cepat dan akurat.
* Mengurangi kesalahan pencatatan administrasi yang dilakukan secara manual.

## 3. Ruang Lingkup Sistem

Sistem mencakup pengelolaan data siswa, data orang tua, data kelas, proses pendaftaran siswa baru, pencatatan pembayaran biaya pendaftaran dan SPP, serta pembuatan laporan administrasi. Sistem tidak mencakup proses kegiatan belajar mengajar maupun penilaian akademik siswa.

## 4. Pemangku Kepentingan (Stakeholders)

* Siswa → Peserta didik yang terdaftar di PAUD.
* Orang Tua/Wali → Pihak yang melakukan pendaftaran dan pembayaran biaya pendidikan.
* Admin/Tata Usaha → Pengelola data siswa, kelas, dan pembayaran.
* Guru → Pihak yang menerima informasi data siswa berdasarkan kelas.
* Kepala PAUD → Pihak yang memanfaatkan laporan administrasi untuk pengambilan keputusan.

## 5. Kebutuhan Fungsional

* Sistem dapat mencatat data pendaftaran siswa baru.
* Sistem dapat menyimpan data orang tua atau wali siswa.
* Sistem dapat mengelola data kelas dan penempatan siswa.
* Sistem dapat mencatat pembayaran biaya pendaftaran.
* Sistem dapat mencatat pembayaran SPP siswa.
* Sistem dapat menampilkan status pembayaran siswa.
* Sistem dapat menghasilkan laporan data siswa dan pembayaran.
* Sistem dapat melakukan pencarian data siswa berdasarkan nama atau nomor induk.

# ERD

### Orang_Tua

Menyimpan data orang tua atau wali siswa seperti nama, alamat, nomor telepon, dan pekerjaan sebagai pihak yang bertanggung jawab terhadap siswa.

### Siswa

Menyimpan data siswa seperti nomor induk, nama siswa, tanggal lahir, jenis kelamin, dan alamat.

### Kelas

Menyimpan data kelas yang tersedia di PAUD, seperti Kelompok Bermain, TK A, atau TK B.

### Pendaftaran

Mencatat proses pendaftaran siswa baru beserta tanggal pendaftaran dan biaya pendaftaran yang harus dibayarkan.

### Pembayaran

Menyimpan data transaksi pembayaran siswa, baik pembayaran biaya pendaftaran maupun pembayaran SPP.

### Metode_Pembayaran

Menyimpan informasi metode pembayaran yang digunakan, seperti Tunai, Transfer Bank, atau QRIS.

## Penjelasan Relasi

* Satu Orang_Tua dapat memiliki satu atau lebih Siswa.
* Satu Siswa terdaftar pada satu Kelas.
* Satu Siswa memiliki satu data Pendaftaran.
* Satu Siswa dapat melakukan banyak Pembayaran selama masa belajar.
* Satu Pembayaran menggunakan satu Metode_Pembayaran.
* Satu Kelas dapat memiliki banyak Siswa.

### Penjelasan Relasi Jika Ditanya Dosen

"Satu orang tua dapat memiliki beberapa anak yang terdaftar sebagai siswa di PAUD. Setiap siswa ditempatkan pada satu kelas tertentu. Saat pertama kali masuk, siswa melakukan satu proses pendaftaran. Selama bersekolah, siswa dapat melakukan banyak pembayaran seperti biaya pendaftaran dan SPP bulanan. Setiap transaksi pembayaran menggunakan satu metode pembayaran tertentu. Sementara itu, satu kelas dapat diisi oleh banyak siswa."
