  <h1>HRIS - Human Resource Information System</h1>

  <p>Sistem informasi sumber daya manusia (HRIS) berbasis web yang dibangun menggunakan Laravel. Proyek ini mencakup manajemen data karyawan, kehadiran, penggajian, dan permintaan cuti.</p>

  <h2>📌 Fitur</h2>
  <ul>
    <li>Manajemen data karyawan</li>
    <li>Sistem absensi (presensi)</li>
    <li>Permintaan cuti (leave request)</li>
    <li>Penggajian (payroll) otomatis</li>
    <li>Manajemen departemen dan peran (roles)</li>
    <li>Seeder dan migrasi database lengkap</li>
  </ul>

  <h2>🛠️ Teknologi</h2>
  <ul>
    <li>PHP 8+</li>
    <li>Laravel 10+</li>
    <li>MySQL</li>
    <li>Composer</li>
    <li>XAMPP / Laravel Sail (opsional)</li>
  </ul>

  <h2>🚀 Instalasi</h2>

  <h3>1. Clone proyek</h3>
  <pre><code>git clone https://github.com/username/hris.git
cd hris</code></pre>

  <h3>2. Install dependency</h3>
  <pre><code>composer install
npm install &amp;&amp; npm run dev</code></pre>

  <h3>3. Salin file konfigurasi</h3>
  <pre><code>cp .env.example .env
php artisan key:generate</code></pre>

  <h3>4. Atur koneksi database</h3>
  <p>Edit file <code>.env</code> dan sesuaikan dengan database lokal kamu:</p>
  <pre><code>DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=hris
DB_USERNAME=root
DB_PASSWORD=</code></pre>

  <h3>5. Migrasi dan seeder</h3>
  <pre><code>php artisan migrate --seed</code></pre>

  <h3>6. Jalankan server lokal</h3>
  <pre><code>php artisan serve</code></pre>
  <p>Akses aplikasi di <a href="http://localhost:8000">http://localhost:8000</a></p>

  <h2>✅ Catatan</h2>
  <p>Jika kamu mengalami error saat menjalankan <code>migrate:refresh</code>, pastikan tidak ada constraint yang terblokir. Cek ulang urutan <code>Schema::dropIfExists</code> di fungsi <code>down()</code> atau kosongkan database secara manual sebelum migrasi ulang.</p>

  <h2>📝 Lisensi</h2>
  <p>Proyek ini dirilis di bawah lisensi MIT.</p>
