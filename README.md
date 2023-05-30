<a href="https://github.com/togiberlin/ui-ux-designer-roadmap">Roadmap UI/UX</a>

1. Jelaskan pengertian Basis Data dan Sistem Basis Data ?
- Basis data Merupakan kumpulan data yang `saling berhubungan` (punya relasi),
Relasi ditunjukan dengan `kunci` (key) dari tiap file yang ada
- Sistem basis data merupakan sistem yang terdiri dari kumpulan file atau tabel yang saling berhubungan dan memungkinkan beberapa pemakai mengakses dan memanipulasinya, Istilah sistem basis data : merupakan lingkup yang lebih luas daripada basis data

2. Jelaskan komponen-komponen dari Sistem Basis Data?
- Pemakai (*User*)
- Programmer Aplikasi (*Application Programmer*) : pemakai yang berinteraksi dengan basis data melalui `DML` yang disertakan dalam program yang ditulis dalam bahasa pemrograman
- User Mahir (*Casual User*) : Pemakai menggunakan query untuk akses data
- User Umum (*Naive User*) : Pemakai yang berinteraksi dengan sistem basis data melalui pemanggilan satu program aplikasi permanen
- User Khusus (*Specialized User*) : pemakai yang menulis aplikasi basis data non konvensional untuk keperluan khusus, seperti untuk aplikasi sistem pakar, pengolahan citra dll.

3. Jelaskan Komponen Dari Hirarki Basis Data dan Gambarkan Piramidanya?
- `Bit` , suatu sistem angka biner yang terdiri atas dua macam nilai saja yaitu, 0 dan 1.
- `Karakter`, merupakan data yang paling kecil yang membuat sebuah data.
- `Field`, unit terkecil yang disebut data. merupakan sekumpulan byte yang memiliki makna.
- `Record`, kumpulan item yang secara logis saling berhubungan. 
- `File`, yaitu bagian yang terdiri dari record yang sama.
- `Database`, kumpulan file-file yang secara logis dan digunakan secara rutin pada operasi-operasi sistem informasi manajemen.
<div style="margin: 0 0.8em">

| NO | PIRAMID |
|:--:|:-------:|
| 1  | BIT |
| 2 | Karakter |
| 3 | Field |
| 4 | Record |
| 5 | File |
| 6 | Database |

</div>

4. Sebutkan Operasi yang ada pada basis data, Tujuan Basis Data?
- **Operasi Basis Data :**
- Pembuatan Basis Data baru
- Penghapusan Basis Data
- Pembuatan Tabel Baru
- Penghapusan Tabel
- Pengisian/Penambahan Data Baru
- Pengambilan Data
- Pengubahan Data
- Penghapusan Data
- **Tujuan Basis Data :**
- Kecepatan dan Kemudahan (*Speed*)
- Efisiensi ruang penyimpanan (*Space*)
- Keakuratan (*Accuracy*)
- Ketersediaan (*Availability*)
- Kelengkapan (*Completeness*)
- Keamanan (*Security*)
- Kebersamaan Pemakai (*Sharebility*)

5. Sebutkan contoh penerapan basis data dari berbagai perusahaan/organisasi minimal 10?
- Perusahaan E-commerce: Basis data digunakan untuk menyimpan informasi produk, data pelanggan, dan riwayat transaksi.

- Bank: Basis data digunakan untuk menyimpan informasi nasabah, rekening, transaksi keuangan, dan riwayat kredit.

- Rumah Sakit: Basis data digunakan untuk menyimpan informasi pasien, catatan medis, jadwal dokter, dan inventaris obat.

- Perusahaan Telekomunikasi: Basis data digunakan untuk menyimpan informasi pelanggan, nomor telepon, riwayat panggilan, dan penggunaan data.

- Pemerintah Daerah: Basis data digunakan untuk menyimpan data penduduk, kependudukan, administrasi perizinan, dan informasi publik.

- Perusahaan Transportasi: Basis data digunakan untuk menyimpan informasi penerbangan, jadwal kereta, reservasi tiket, dan data kargo.

- Universitas: Basis data digunakan untuk menyimpan data mahasiswa, jadwal kuliah, informasi akademik, dan catatan keuangan.

- Perusahaan Manufaktur: Basis data digunakan untuk menyimpan informasi produksi, inventaris barang, data pemasok, dan analisis kualitas.

- Perusahaan Asuransi: Basis data digunakan untuk menyimpan informasi polis, klaim asuransi, data premi, dan riwayat klaim.

- Perusahaan Logistik: Basis data digunakan untuk menyimpan informasi pengiriman, rute pengiriman, data pelanggan, dan status pengiriman.

- Perusahaan Perhotelan: Basis data digunakan untuk menyimpan informasi pemesanan kamar, riwayat tamu, inventaris hotel, dan data keuangan.

- Perusahaan Ritel: Basis data digunakan untuk menyimpan informasi inventaris produk, data pelanggan, transaksi penjualan, dan analisis penjualan.

6. Buatlah database yang anda ketahui mulai dari ERD nya , tabel dan struktur tabel?

<div style="margin: 0 0.8em">

Nama database: article_db
<br>
Nama Tabel : users

|  FIELD   |    TYPE     | NULL | KEY | DEFAULT | KETERANGAN  |
|:--------:|:-----------:| :-: |:---:| :-: |:-----------:|
| username | varchar(12) | NO | PRI | NULL | PRIMARY KEY |
| email |   varchar(55) | NO | | NULL |             |
| password | varchar(255) | NO | | NULL |             |\

Nama Tabel : categories

| FIELD | TYPE | NULL | KEY | DEFAULT | KETERANGAN |
|:-:|:-:| :-: |:---:| :-: |:----------:|
| category_id | int(2) | NO | PRI | NULL | PRIMARY KEY|
| category | varchar(55) | NO | | NULL | |

Nama Tabel : articles

|    FIELD     | TYPE | NULL | KEY | DEFAULT | KETERANGAN  |
|:------------:|:-:| :-: |:---:| :-: |:-----------:|
|  article_id  | varchar(255) | NO | PRI | NULL |             |
|  user_name   | varchar(12) | NO | MUL | NULL | FOREIGN KEY |
|     head     | varchar(255) | NO |     | NULL |             |
| descriptions | text | NO |     | NULL |             |
| category_id  | int(2) | NO | MUL | NULL | FOREIGN KEY |

</div>
