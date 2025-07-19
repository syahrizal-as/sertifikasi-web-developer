# Materi Sertifikasi Web Developer (Berbasis Laravel)

Disusun untuk membantu peserta mempersiapkan diri menghadapi uji kompetensi berdasarkan 22 unit SKKNI.

## 1. Melaksanakan cutover aplikasi
**Deskripsi:**
Cutover aplikasi adalah proses pemindahan dari sistem lama ke sistem baru secara penuh. Dalam konteks Laravel, ini bisa berkaitan dengan proses deployment aplikasi Laravel ke server produksi.

**Materi yang Harus Dikuasai:**
- Pengertian cutover dan proses deployment
- Langkah-langkah deployment Laravel (env, migrate, cache, queue, dll)
- Backup dan rollback
- Downtime management

**Contoh Implementasi Laravel:**
Contoh perintah untuk deployment Laravel:
```bash
php artisan migrate --force
php artisan config:cache
php artisan route:cache
```

**Latihan:**
- Jelaskan proses cutover aplikasi
- Lakukan simulasi deployment aplikasi Laravel ke server lokal

---

## 2. Melakukan debugging
**Deskripsi:**
Debugging adalah proses menemukan dan memperbaiki error/bug pada aplikasi. Laravel menyediakan berbagai tools seperti debugging dengan Laravel Telescope, Log, atau Xdebug.

**Materi yang Harus Dikuasai:**
- Konsep debugging
- Debugging tools di Laravel: Log, Dump, Debugbar, Telescope
- Menangani exception dan logging

**Contoh Implementasi Laravel:**
Contoh debugging di Laravel:
```php
Log::info('User data', ['user' => $user]);
dd($user); // Dump and Die
```

**Latihan:**
- Gunakan Laravel Debugbar untuk memantau query
- Temukan dan perbaiki bug pada fitur login

---

