# Alur Pembelian ERM Offline

## Prinsip

- Website menjelaskan produk, paket, dan cara membeli.
- WhatsApp dipakai untuk demo, rekomendasi paket, pembayaran, dan aktivasi.
- Installer tidak tersedia sebagai download publik.
- Aplikasi penuh hanya aktif dengan license key berbasis device fingerprint.

## Status Lead

- `Demo`
- `Pilih Paket`
- `Menunggu Pembayaran`
- `Lunas`
- `Installer Dikirim`
- `Menunggu Aktivasi`
- `Aktif`
- `Pindah Perangkat`

## SOP End-to-End

1. Lead masuk dari website melalui WhatsApp.
2. Tanyakan jenis praktik, jumlah perangkat, pencatatan saat ini, dan kebutuhan kasir/antrean.
3. Jadwalkan demo 15 menit memakai data dummy.
4. Setelah demo, rekomendasikan paket dan jelaskan batasan produk.
5. Jika cocok, kirim nominal dan metode pembayaran transfer/QRIS.
6. Setelah bukti pembayaran diterima, validasi manual.
7. Catat pembayaran di `lead-tracker.csv`.
8. Kirim installer privat, checksum SHA-256, dan panduan instalasi.
9. Minta device fingerprint/request code dari aplikasi.
10. Buat atau siapkan license key sesuai paket dan perangkat.
11. Kirim license key dan bantu aktivasi.
12. Catat status `Aktif`, versi installer, fingerprint, dan referensi license key.

## Catatan Keamanan

- Jangan kirim secret, private key, atau generator lisensi melalui repo publik.
- Jangan taruh link installer publik di website.
- Jangan klaim SATUSEHAT/cloud/Android sebagai fitur siap pakai.
- Gunakan data dummy saat demo.
- Simpan arsip installer per versi untuk support.
