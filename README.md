# PharmaSys

PharmaSys adalah sistem manajemen apotek berbasis web yang dibangun menggunakan Laravel dan PostgreSQL. Sistem ini dirancang untuk membantu pengelolaan produk, transaksi penjualan, pembelian, laporan, serta manajemen pengguna di lingkungan apotek.

## Fitur Utama

- **Login & Role Management**  
  Sistem mendukung login untuk Admin dan Kasir. Admin dapat mengakses seluruh fitur, sedangkan Kasir hanya fitur terkait penjualan.

- **Dashboard**  
  Menampilkan ringkasan data penting, grafik statistik penjualan bulanan, dan informasi terkini.

- **Manajemen Kategori Produk**  
  Tambah, edit, dan hapus kategori produk.

- **Manajemen Produk**  
  Tambah, edit, hapus produk, serta monitoring stok, produk kadaluarsa, dan out-stock.

- **Pembelian (Purchase)**  
  Proses pembelian produk dari supplier, update stok otomatis.

- **Penjualan (Sale) & Pembayaran**  
  Proses transaksi penjualan, pembayaran, dan pencetakan struk.

- **Supplier**  
  Manajemen data supplier.

- **Laporan (Reports)**  
  Laporan penjualan dan pembelian dalam bentuk tabel dan grafik.

- **Statistik Penjualan**  
  Grafik penjualan bulanan pada dashboard.

- **Manajemen Pengguna & Hak Akses**  
  Pengelolaan akun, role, dan permission pengguna.

- **Profile & Settings**  
  Update profil pengguna dan pengaturan sistem.

> **Catatan:** Fitur backup saat ini dinonaktifkan.

## Instalasi

1. **Clone repository**
   ```bash
   git clone <repo-url>
   cd PharmacyMS-Laravel-3
   ```

2. **Install dependencies**
   ```bash
   composer install
   npm install && npm run dev
   ```

3. **Copy file environment**
   ```bash
   cp .env.example .env
   ```

4. **Konfigurasi database di file `.env`**
   ```
   DB_CONNECTION=pgsql
   DB_HOST=127.0.0.1
   DB_PORT=5432
   DB_DATABASE=pharmasys_db
   DB_USERNAME=postgres
   DB_PASSWORD=postgres
   ```

5. **Generate key**
   ```bash
   php artisan key:generate
   ```

6. **Migrasi database**
   ```bash
   php artisan migrate
   ```

7. **Jalankan server**
   ```bash
   php artisan serve
   ```

8. **Akses aplikasi**
   Buka browser ke [http://127.0.0.1:8000](http://127.0.0.1:8000)

## Kontribusi

Silakan buat issue atau pull request untuk perbaikan dan pengembangan fitur.
