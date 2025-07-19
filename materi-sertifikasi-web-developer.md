# Materi Sertifikasi Web Developer (Berbasis Laravel)

Berikut ini adalah materi lengkap 22 unit berdasarkan SKKNI, dengan pendekatan Laravel:

## 1. Melaksanakan cutover aplikasi

**Deskripsi:** Cutover aplikasi adalah proses pemindahan dari sistem lama ke sistem baru secara penuh. Dalam konteks Laravel, ini bisa berkaitan dengan proses deployment aplikasi Laravel ke server produksi.

**Materi yang Harus Dikuasai:**

- Pengertian cutover dan proses deployment
- Langkah-langkah deployment Laravel (env, migrate, cache, queue, dll)
- Backup dan rollback
- Downtime management

**Contoh Implementasi Laravel:**

```bash
php artisan migrate --force
php artisan config:cache
php artisan route:cache
```

**Latihan:**

- Jelaskan proses cutover aplikasi
- Lakukan simulasi deployment aplikasi Laravel ke server lokal

---

## 2. Melakukan pemantauan resource yang digunakan aplikasi

**Deskripsi:** Unit ini membahas tentang melakukan pemantauan resource yang digunakan aplikasi dalam pengembangan perangkat lunak. Pendekatan yang digunakan adalah dengan framework Laravel.

**Materi yang Harus Dikuasai:**

- Konsep pemantauan resource
- Studi kasus dalam proyek Laravel
- Implementasi teknis dengan Laravel

**Contoh Implementasi Laravel:**

```php
// Contoh penggunaan Laravel Telescope atau Laravel Debugbar untuk memantau resource
```

**Latihan:**

- Jelaskan langkah-langkah melakukan pemantauan resource dalam Laravel
- Buatkan simulasi atau studi kasus monitoring penggunaan CPU/memory pada Laravel

---

## 3. Melakukan debugging

**Deskripsi:** Debugging adalah proses menemukan dan memperbaiki error/bug pada aplikasi. Laravel menyediakan berbagai tools seperti debugging dengan Laravel Telescope, Log, atau Xdebug.

**Materi yang Harus Dikuasai:**

- Konsep debugging
- Debugging tools di Laravel: Log, Dump, Debugbar, Telescope
- Menangani exception dan logging

**Contoh Implementasi Laravel:**

```php
Log::info('User data', ['user' => $user]);
dd($user); // Dump and Die
```

**Latihan:**

- Gunakan Laravel Debugbar untuk memantau query
- Temukan dan perbaiki bug pada fitur login

---

## 4. Melaksanakan pengujian oleh pengguna (UAT)

**Deskripsi:** Unit ini membahas tentang melaksanakan pengujian oleh pengguna (UAT) dalam pengembangan perangkat lunak. Pendekatan yang digunakan adalah dengan framework Laravel.

**Materi yang Harus Dikuasai:**

- Konsep UAT dan validasi fitur
- Studi kasus UAT pada aplikasi Laravel
- Implementasi dengan Laravel dan Inertia.js

**Contoh Implementasi Laravel:**

```php
// Simulasi testing fitur oleh user menggunakan fitur Test di Laravel
```

**Latihan:**

- Susun checklist UAT untuk fitur login
- Simulasikan UAT menggunakan seeder dan test di Laravel

---

## 5. Mengelola risiko keamanan Informasi

**Deskripsi:** Unit ini membahas tentang pengelolaan risiko keamanan informasi. Dalam Laravel, pengamanan meliputi input validation, authentication, authorization, dan secure deployment.

**Materi yang Harus Dikuasai:**

- Keamanan form dan data
- Middleware dan validasi input
- Laravel Sanctum/Passport

**Contoh Implementasi Laravel:**

```php
$request->validate([
    'email' => 'required|email',
    'password' => 'required|min:6',
]);
```

**Latihan:**

- Analisa celah XSS dan SQL Injection di aplikasi
- Terapkan middleware untuk role tertentu

---

## 6. Menggunakan SQL

**Deskripsi:** Unit ini membahas tentang penggunaan SQL dalam pengembangan web menggunakan Laravel.

**Materi yang Harus Dikuasai:**

- Konsep penggunaan SQL
- Studi kasus dalam Laravel
- Penerapan teknis menggunakan Laravel (Controller, Model, Middleware, Testing, dll)

**Contoh Implementasi Laravel:**

```php
$data = DB::select('SELECT * FROM users WHERE email = ?', [$email]);
```

**Latihan:**

- Buat simulasi penggunaan SQL dalam Laravel
- Jelaskan proses atau langkah penerapannya dalam Laravel

---

## 7. Menerapkan alert notification jika aplikasi bermasalah

**Deskripsi:** Unit ini membahas tentang penerapan notifikasi jika aplikasi bermasalah dalam Laravel.

**Materi yang Harus Dikuasai:**

- Konsep notifikasi dan alert
- Studi kasus monitoring dalam Laravel
- Penerapan notifikasi via email, Slack, Telegram

**Contoh Implementasi Laravel:**

```php
Notification::route('mail', 'admin@example.com')
    ->notify(new App\Notifications\ErrorNotification($error));
```

**Latihan:**

- Simulasikan error monitoring
- Kirim notifikasi ke admin saat terjadi exception

---

## 8. Melakukan identifikasi library, komponen atau framework yang diperlukan

**Deskripsi:** Unit ini membahas bagaimana menentukan library dan framework yang sesuai.

**Materi yang Harus Dikuasai:**

- Composer dan dependency management
- Evaluasi library

**Contoh Implementasi Laravel:**

```bash
composer require laravel/sanctum
```

**Latihan:**

- Identifikasi library untuk autentikasi
- Instal dan dokumentasikan penggunaannya

---

## 9. Melakukan migrasi ke teknologi baru

**Deskripsi:** Menerapkan perubahan teknologi, seperti upgrade Laravel atau pindah ke stack baru.

**Materi yang Harus Dikuasai:**

- Upgrade Laravel
- Pindah ke Inertia.js atau Livewire

**Contoh Implementasi Laravel:**

```bash
composer update
```

**Latihan:**

- Upgrade Laravel dari versi 9 ke 10

---

## 10. Melakukan pembaharuan perangkat lunak

**Deskripsi:** Unit ini membahas proses update software

**Materi yang Harus Dikuasai:**

- Versioning dan update dependencies
- Backup sebelum update

**Contoh Implementasi Laravel:**

```bash
composer outdated
composer update vendor/package
```

**Latihan:**

- Perbarui dependency yang tidak kompatibel

---

## 11. Memberikan petunjuk teknis kepada pelanggan

**Deskripsi:** Menulis dokumentasi teknis aplikasi Laravel

**Materi yang Harus Dikuasai:**

- Markdown
- Contoh dokumentasi API

**Contoh Implementasi Laravel:**

```php
// OpenAPI/Swagger atau Postman collection
```

**Latihan:**

- Buat README dan dokumentasi endpoint

---

## 12. Menerapkan pemrograman multimedia

**Deskripsi:** Menangani file gambar, audio, dan video

**Materi yang Harus Dikuasai:**

- Upload file
- Manipulasi gambar dengan Intervention Image

**Contoh Implementasi Laravel:**

```php
$image = Image::make($request->file('photo'))->resize(300, 300);
```

**Latihan:**

- Upload dan resize gambar user

---

## 13. Menentukan arsitektur perangkat keras

**Deskripsi:** Menentukan kebutuhan infrastruktur

**Materi yang Harus Dikuasai:**

- Shared hosting, VPS, Cloud
- Load balancing dan scaling

**Latihan:**

- Bandingkan 2 arsitektur hosting Laravel

---

## 14. Mengelola proyek secara terintegrasi (project integration management)

**Deskripsi:** Manajemen integrasi tim dan alur kerja

**Materi yang Harus Dikuasai:**

- Git, CI/CD, dan branching strategy

**Latihan:**

- Buat workflow CI/CD untuk project Laravel

---

## 15. Menganalisis tools

**Deskripsi:** Analisis tools pengembangan dan monitoring

**Materi yang Harus Dikuasai:**

- Debugbar, Telescope, Sentry

**Latihan:**

- Bandingkan Telescope dan Debugbar

---

## 16. Menganalisis skalabilitas perangkat lunak

**Deskripsi:** Evaluasi kemampuan aplikasi menangani beban besar

**Materi yang Harus Dikuasai:**

- Queue, Cache, Horizon

**Latihan:**

- Simulasi queue dan scaling

---

## 17. Menganalisis dampak perubahan terhadap aplikasi

**Deskripsi:** Uji regresi dan analisis dependensi

**Materi yang Harus Dikuasai:**

- Unit testing dan refactoring

**Latihan:**

- Tambah fitur tanpa rusak fitur lama

---

## 18. Menerapkan pemrograman paralel

**Deskripsi:** Proses paralel dalam Laravel (Queue, Jobs, Broadcasting)

**Latihan:**

- Kirim email massal dengan queue

---

## 19. Mengelola kualitas proyek (project quality management)

**Deskripsi:** Review kode, testing otomatis

**Materi yang Harus Dikuasai:**

- Code Sniffer, PHPUnit

**Latihan:**

- Jalankan test otomatis dan review

---

## 20. Mengimplementasikan algoritma pemrograman

**Deskripsi:** Algoritma dasar dan kompleksitas

**Latihan:**

- Buat sorting manual data Laravel Collection

---

## 21. Menerapkan pemrograman real time

**Deskripsi:** Gunakan WebSocket, Laravel Echo

**Latihan:**

- Buat fitur chat sederhana

---

## 22. Mengelola ruang lingkup proyek (project scope management)

**Deskripsi:** Breakdown fitur, milestone, dan prioritas kerja

**Latihan:**

- Susun daftar backlog dan sprint Laravel

---

