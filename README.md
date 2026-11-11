# HADIR PRO — Versi Awal

Aplikasi absensi berbasis web/PWA, dirancang mobile-first dan dapat dipakai secara lokal/offline setelah pertama kali dibuka melalui server lokal atau hosting HTTPS.

## Fitur yang sudah berfungsi
- Dashboard ringkasan kehadiran.
- Tambah dan hapus anggota.
- Catat absensi masuk/pulang dan status.
- Status terlambat otomatis berdasarkan batas waktu masuk.
- Riwayat dan filter tanggal/status.
- Ekspor CSV.
- Backup dan restore JSON.
- Tema gelap.
- Penyimpanan lokal browser (localStorage).
- Service worker untuk cache aplikasi.

## Cara menjalankan
Cara termudah: ekstrak ZIP, lalu unggah isi folder ke hosting statis yang mendukung HTTPS. Untuk uji lokal di komputer, jalankan server HTTP dari folder ini, misalnya:
`python -m http.server 8000`
Lalu buka `http://localhost:8000`.

Di Android, buka alamat HTTPS melalui Chrome lalu pilih menu **Tambahkan ke layar utama / Install app**.

## Catatan penting
Ini adalah MVP lokal satu perangkat, bukan sistem multiuser online. Data tersimpan di browser/perangkat yang digunakan dan tidak otomatis dibagikan ke admin atau perangkat lain. GPS, QR dinamis, selfie, login multiuser, persetujuan izin/cuti, backend, sinkronisasi, dan laporan PDF/Excel belum diimplementasikan. Jangan gunakan untuk payroll atau keputusan kepegawaian resmi sebelum menambahkan backend, autentikasi, audit, backup terpusat, dan pengujian keamanan.

Ekspor cadangan JSON secara berkala. Menghapus data browser dapat menghapus data aplikasi.
