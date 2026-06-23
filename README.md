## Pengembang

# Nama : Keiveen Aldiandra
## NPM: 2408107010085

---

# Sistem Pengaduan Kampus

## Deskripsi Aplikasi

Sistem Pengaduan Kampus adalah aplikasi web berbasis Laravel yang digunakan untuk memudahkan mahasiswa dalam menyampaikan pengaduan terkait fasilitas, layanan, maupun kegiatan akademik di lingkungan kampus. Aplikasi ini memungkinkan pengguna mengirim pengaduan, melihat status pengaduan, serta membantu admin dalam mengelola dan menindaklanjuti laporan yang masuk.

---

## Fitur Utama

* Login dan autentikasi pengguna
* Manajemen pengguna
* Manajemen kategori pengaduan
* Pembuatan pengaduan
* Melihat daftar pengaduan
* Manajemen status pengaduan
* Dashboard admin
* Sistem role dan permission

---

## Teknologi yang Digunakan

### Backend

* PHP
* Laravel Framework

### Frontend

* Blade Template Engine
* HTML
* CSS
* JavaScript
* Bootstrap
* Vite

### Database

* MySQL

### Tools

* Composer
* Node.js
* NPM
* Git
* GitHub
* XAMPP

---

## Struktur Database

Tabel utama yang digunakan:

* users
* permissions
* roles
* kategoris
* pengaduans

Migration yang tersedia:

* create_users_table
* create_cache_table
* create_jobs_table
* create_permission_tables
* create_kategoris_table
* create_pengaduans_table

---

## Persyaratan Sistem

Sebelum menjalankan aplikasi, pastikan telah menginstal:

* PHP 8.x
* Composer
* Node.js
* NPM
* MySQL
* XAMPP
* Git

---

## Cara Instalasi

### 1. Clone Repository

```bash
git clone https://github.com/keiveenaldiandra/UAS-PBW-Pengaduan-Kampus.git
```

Masuk ke folder project:

```bash
cd UAS-PBW-Pengaduan-Kampus
```

---

### 2. Install Dependency Laravel

```bash
composer install
```

Perintah ini akan mengunduh seluruh dependency Laravel dan membuat folder vendor.

---

### 3. Membuat File Environment

```bash
cp .env.example .env
```

---

### 4. Generate Application Key

```bash
php artisan key:generate
```

Jika berhasil akan muncul:

```text
INFO  Application key set successfully.
```

---

### 5. Konfigurasi Database

Buka file:

```text
.env
```

Kemudian ubah konfigurasi database menjadi:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=pengaduan_kampus
DB_USERNAME=root
DB_PASSWORD=
```

---

### 6. Menjalankan MySQL

* Jalankan XAMPP
* Start Apache
* Start MySQL

Pastikan database:

```text
pengaduan_kampus
```

sudah tersedia pada phpMyAdmin.

---

### 7. Membersihkan Cache Konfigurasi

```bash
php artisan config:clear
php artisan cache:clear
```

---

### 8. Verifikasi Koneksi Database

```bash
php artisan migrate:status
```

Jika berhasil, seluruh migration akan berstatus:

```text
Ran
```

---

### 9. Install Dependency Frontend

```bash
npm install
```

Perintah ini akan mengunduh seluruh package JavaScript dan membuat folder node_modules.

---

### 10. Menjalankan Vite

```bash
npm run dev
```

Vite digunakan untuk mengelola asset frontend seperti CSS dan JavaScript selama proses development.

---

### 11. Menjalankan Laravel

Buka terminal baru kemudian jalankan:

```bash
php artisan serve
```

Jika berhasil akan muncul:

```text
INFO Server running on http://127.0.0.1:8000
```

Buka browser dan akses:

```text
http://127.0.0.1:8000
```

---

## Cara Penggunaan

### Admin

* Login ke sistem
* Mengelola kategori pengaduan
* Mengelola data pengguna
* Melihat seluruh pengaduan
* Mengubah status pengaduan
* Mengelola hak akses pengguna

### Pengguna

* Login ke sistem
* Membuat pengaduan
* Melihat daftar pengaduan
* Memantau status pengaduan

---

## Repository GitHub

https://github.com/keiveenaldiandra/UAS-PBW-Pengaduan-Kampus
