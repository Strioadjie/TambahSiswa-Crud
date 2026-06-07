# Aplikasi CRUD Data Siswa

Aplikasi berbasis web sederhana untuk mengelola data siswa. Dibuat menggunakan PHP Native dan MySQL dengan fungsionalitas CRUD (Create, Read, Update, Delete).

## Fitur

* Menambahkan data siswa baru.
* Menampilkan daftar semua siswa.
* Melihat detail informasi spesifik siswa.
* Mengubah informasi data siswa.
* Menghapus data siswa.

## Kebutuhan Sistem

* Web Server lokal seperti XAMPP, WAMP, atau serupa.
* PHP versi 7.x atau 8.x.
* MySQL Database.

## Panduan Instalasi

1. Pindahkan folder proyek ini ke dalam direktori root server web Anda (contohnya folder `htdocs` jika Anda menggunakan XAMPP).
2. Jalankan Apache dan MySQL pada panel kontrol server web lokal Anda.
3. Buka phpMyAdmin (biasanya dapat diakses melalui `http://localhost/phpmyadmin`).
4. Buat database baru dengan nama `crud_app`.
5. Import file `database.sql` yang ada pada folder ini ke dalam database `crud_app` yang baru saja Anda buat.
6. Buka browser dan akses aplikasi melalui `http://localhost/nama-folder-proyek` (sesuaikan `nama-folder-proyek` dengan nama folder Anda).

## Konfigurasi Database

Secara bawaan aplikasi ini menggunakan kredensial default dari XAMPP. Jika Anda memiliki pengaturan kredensial database yang berbeda, Anda dapat mengubahnya di dalam file `koneksi.php`:

```php
$con = mysqli_connect("localhost", "username_anda", "password_anda", "crud_app");
```

## Struktur File Utama

* `index.php` : Halaman utama yang menampilkan daftar seluruh siswa.
* `tambah_siswa.php` : Halaman form untuk memasukkan data siswa baru.
* `detail_data_siswa.php` : Halaman untuk melihat detail data satu siswa.
* `edit_data_siswa.php` : Halaman form untuk memperbarui data siswa.
* `code.php` : File yang memproses logika atau query database (Tambah, Ubah, Hapus).
* `koneksi.php` : Konfigurasi koneksi ke server database MySQL.
* `database.sql` : Skema struktur database dan tabel.
