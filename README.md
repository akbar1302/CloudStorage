# Cloud Storage Sederhana dengan Google Drive API

## Deskripsi Proyek
Proyek ini merupakan tugas akhir mata kuliah Pemrograman Jaringan yang bertujuan untuk membuat website cloud storage sederhana. Website ini terintegrasi dengan Google Drive menggunakan Google Drive API dan dilengkapi fitur:

- Login menggunakan akun Google
- Upload file ke Google Drive
- Tabel data file yang mencakup informasi:
  - Nama file
  - Ukuran file
  - Jenis file
  - Tanggal dan waktu upload
- Tombol download dan hapus file

## Teknologi yang Digunakan
1. **Frontend:**
   - HTML
   - CSS (tema bertema cloud)
   - JavaScript
2. **Backend:**
   - PHP
   - MySQL (untuk menyimpan token sesi dan data terkait login)
3. **Composer**
   - Untuk mengelola library vendor (Google API Client Library for PHP).
4. **Google Drive API**

## Cara Instalasi
1. **Clone Repository**
   ```bash
   git clone <repository-url>
   cd CloudStorage
   ```

2. **Instalasi Composer**
   Pastikan Composer telah terinstal. Jika belum, unduh dari [situs resmi Composer](https://getcomposer.org/).
   
   Jalankan perintah berikut untuk menginstal library yang diperlukan:
   ```bash
   composer install
   ```

3. **Konfigurasi Google API**
   - Buat project di [Google Cloud Console](https://console.cloud.google.com/).
   - Aktifkan Google Drive API.
   - Buat kredensial OAuth 2.0 dan unduh file `credentials.json`.
   - Letakkan file `credentials.json` di root proyek.

4. **Konfigurasi Database**
   - Buat database MySQL baru.
   - Import file `database.sql` (jika ada) untuk membuat tabel yang diperlukan.
   - Update file konfigurasi database di proyek Anda (contoh: `config.php`).

5. **Jalankan Server Lokal**
   Gunakan server lokal seperti XAMPP atau Laravel Valet:
   ```bash
   php -S localhost:8000
   ```

6. **Akses Website**
   Buka browser Anda dan akses:
   ```
   http://localhost:8000
   ```

## Fitur
1. **Login Google:**
   Pengguna dapat masuk menggunakan akun Google mereka.
2. **Dashboard:**
   - Upload file ke Google Drive.
   - Melihat informasi file yang telah diunggah.
   - Download dan hapus file.

## Struktur Folder
- `assets/`: File CSS, JavaScript, dan gambar tema.
- `vendor/`: Library yang dikelola oleh Composer.
- `config/`: File konfigurasi seperti database.
- `src/`: File PHP utama untuk fitur login, upload, dan pengelolaan file.

## Catatan
- Pastikan koneksi internet aktif untuk menggunakan Google API.
- Jangan lupa menyimpan `credentials.json` dengan aman, karena file ini mengandung informasi sensitif.

## Kontribusi
Proyek ini merupakan tugas individu, kontribusi dari pihak luar tidak diperlukan.

## Lisensi
Proyek ini hanya untuk keperluan akademik dan tidak untuk didistribusikan atau digunakan secara komersial.
