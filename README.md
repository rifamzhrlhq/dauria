# Dauria

Panduan singkat untuk menjalankan proyek **Dauria** di komputer lokal setelah `git clone`.

---

## Langkah Setup Wajib

1. **Clone Repositori & Masuk Folder**
   git clone https://github.com/rifamzhrlhq/dauria.git
   cd dauria

2. **Install Dependencies (Composer)**
   composer install

3. **Buat File Environment (.env)**
   - macOS / Linux: `cp .env.example .env`
   - Windows: `copy .env.example .env`

4. **Generate Key**
   php artisan key:generate

5. **Migrasi Database** (ini buat nanti jadi bisa diabaikan dulu aja yah)
   (Pastikan database `dauria_db` sudah dibuat di MySQL/XAMPP, lalu jalankan)
   php artisan migrate 

6. **Jalankan Server**
   php artisan serve

Buka browser dan akses: [http://127.0.0.1:8000](http://127.0.0.1:8000)