# 📚 Web Bookstore - Sistem Manajemen & Toko Buku Native PHP

![PHP](https://img.shields.io/badge/PHP-Native-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Web Bookstore adalah aplikasi berbasis **PHP Native** dan **MySQL** yang dirancang untuk transaksi penjualan buku digital/fisik, pengolahan pesanan, manajemen saldo (*top-up*), serta panel admin interaktif dengan antarmuka yang dinamis.

---

## ✨ Fitur Unggulan

### 👨‍💻 **Fitur Pengguna (User)**
- **Katalog & Navigasi**: Pencarian cepat (*Live Search*) dan katalog produk buku.
- **Top-Up Saldo**: Pengajuan pengisian saldo untuk pembayaran pesanan.
- **Transaksi & Checkout**: Alur pembelian buku langsung dengan rekap pemesanan.
- **Autentikasi & Profile**: Fitur registrasi, login, reset password, dan dashboard user.

### 🛡️ **Fitur Administrator (Admin)**
- **CRUD Data Buku**: Tambah, edit, dan hapus data buku lengkap dengan *live preview* gambar cover.
- **Kelola Pemesanan**: Konfirmasi dan pembaruan status pesanan pelanggan.
- **Verifikasi Top-Up**: Pengelolaan masuknya saldo pengajuan dari user.
- **Interaktivitas Tabel**: Sortir header tabel secara dinamis (*Sortir Table Head*).
- **UI Responsive**: Menu navigasi bilah samping (*Burger Sidebar*) yang fleksibel di berbagai layar.

---

## 📂 Struktur Berkas (File Structure)

```text
Web-Bookstore/
├── img/                    # Asset gambar cover buku & UI
├── admin_pesanan.php       # Panel pengelolaan pesanan oleh Admin
├── checkout.php            # Halaman konfirmasi & pembayaran pesanan
├── dashboard.php           # Routing/Halaman utama dashboard
├── dashboard_admin.php     # Panel kontrol utama Administrator
├── dashboard_user.php      # Panel utama akun pengguna
├── edit_buku.php           # Form sunting data & cover buku
├── footer.php              # Komponen bagian bawah web (Footer)
├── hapus_buku.php          # Skrip eksekusi penghapusan buku
├── header.php              # Komponen bagian atas web (Header & Navbar)
├── index.php               # Halaman utama (Landing Page / Katalog)
├── kelola_pemesanan.php    # Pemrosesan status transaksi pesanan
├── koneksi.php             # Skrip konfigurasi koneksi MySQL
├── konten_pemesanan.php    # Tampilan riwayat & rincian pesanan
├── konten_pemesanan.txt    # Catatan/Log skrip pemesanan
├── konten_topup.php        # Modul pengisian & konfirmasi saldo
├── login.php               # Halaman masuk akun
├── logout.php              # Skrip keluar sistem / Hapus session
├── register.php            # Halaman pendaftaran akun baru
├── reset.php               # Halaman reset kata sandi
├── scriptmodal.js          # Skrip JS untuk Modal interaktif & Live Search
├── tambah_buku.php         # Form penambahan buku baru
└── database.sql            # Skrip skema & data awal basis data

🚀 Panduan Penggunaan & Instalasi LokalPrasyaratWeb Server Lokal (XAMPP, Laragon, atau WAMP)PHP versi 7.4 ke atasDatabase Engine MySQL / MariaDBLangkah InstalasiClone RepositoriBashgit clone [https://github.com/username-anda/Web-Bookstore.git](https://github.com/username-anda/Web-Bookstore.git)
Pindahkan folder proyek ini ke dalam direktori htdocs (XAMPP) atau www (Laragon).Impor Basis DataBuka browser dan masuk ke phpMyAdmin (http://localhost/phpmyadmin).Buat database baru bernama web_bookstore.Impor berkas database.sql ke dalam database tersebut.Konfigurasi KoneksiBuka berkas koneksi.php dan pastikan kredensial sesuai dengan server lokal Anda:PHP$host = "localhost";
$user = "root";
$pass = "";
$db   = "web_bookstore";

$koneksi = mysqli_connect($host, $user, $pass, $db);
Jalankan AplikasiBuka browser dan akses alamat berikut:Plaintexthttp://localhost/Web-Bookstore
🔑 Kredensial Testing DefaultAksesUsernamePasswordAdminadminadmin123UserDapat mendaftar melalui halaman register.php

👨‍💻 PengembangDikembangkan sebagai proyek portofolio aplikasi web berbasis Native PHP.

