# Dauria

Panduan singkat untuk menjalankan proyek **Dauria** di komputer lokal setelah `git clone`.

---

## Tech Stack

* **Backend:** Laravel 13 (PHP 8.2+)
* **Frontend:** React + Inertia.js
* **Styling:** Tailwind CSS / Shadcn UI
* **Database:** MySQL
* **Tooling:** Vite, Composer, Node.js (npm)

## Langkah Setup Wajib

1. **Clone Repositori & Masuk Folder**
   git clone https://github.com/rifamzhrlhq/dauria.git
   cd dauria

2. **Install Dependencies (Composer)**
   composer install

3. **Install Dependensi Frontend (Node.js / React / Inertia / Tailwind)**
   npm install --legacy-peer-deps

4. **Buat File Environment (.env)**
   - macOS / Linux: `cp .env.example .env`
   - Windows: `copy .env.example .env`

5. **Generate Key**
   php artisan key:generate

6. **Generate Application Key**
   php artisan key:generate 
   
7. **Migrasi Database** (ini buat nanti jadi bisa diabaikan dulu aja yah)
   (Pastikan database `dauria_db` sudah dibuat di MySQL/XAMPP, lalu jalankan)
   php artisan migrate

* **Terminal 1 (Server Frontend / Vite Compiler):**
  ```bash
  npm run dev
  ```

* **Terminal 2 (Server Backend / Laravel):**
  ```bash
  php artisan serve
  ```

Buka browser dan akses: [http://127.0.0.1:8000](http://127.0.0.1:8000)