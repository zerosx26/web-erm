# WEB ERM

Static landing page publik untuk produk **MedPraktik**.

## Struktur

- `index.html` - landing page utama.
- `styles.css` - styling responsif clean medical SaaS.
- `script.js` - interaksi kecil untuk menu mobile, smooth scroll, dan galeri screenshot.
- `assets/screenshots/` - visual screenshot-style sementara. Ganti dengan screenshot asli aplikasi MedPraktik saat tersedia.
- `sales/` - materi marketing awal: penawaran, checklist demo, script WhatsApp, dan tracker lead CSV.

## Aktivasi WhatsApp CTA

CTA WhatsApp saat ini memakai nomor:

```js
const WHATSAPP_NUMBER = "6283114869650";
```

Gunakan format internasional tanpa `+`, spasi, atau tanda baca.

## Materi Sales

- `sales/penawaran-erm-offline.md` untuk dikirim setelah calon pembeli tertarik.
- `sales/demo-15-menit-checklist.md` untuk alur demo.
- `sales/script-whatsapp.md` untuk chat awal dan follow-up.
- `sales/alur-pembelian.md` untuk SOP pembelian, pembayaran, delivery, dan aktivasi.
- `sales/template-konfirmasi-pembayaran.md` untuk instruksi transfer/QRIS dan validasi pembayaran.
- `sales/template-pengiriman-installer.md` untuk pengiriman installer privat, checksum, dan aktivasi.
- `sales/lead-tracker.csv` untuk mencatat lead, pembayaran, installer, fingerprint perangkat, dan status aktivasi.

## Deploy GitHub Pages

1. Buat repository publik `zerosx26/web-erm`.
2. Push isi folder ini ke branch `main`.
3. Buka **Settings > Pages**.
4. Pilih **Deploy from a branch**, branch `main`, folder `/root`.
5. URL publik yang diharapkan: `https://zerosx26.github.io/web-erm/`.

## Catatan

- Installer tidak disediakan sebagai download publik di website.
- Pembayaran awal memakai transfer bank/QRIS manual melalui WhatsApp.
- Jangan masukkan source Flutter, license generator, secret, database, atau dokumen internal ke repo ini.
- Klaim cloud, Android companion, dan SATUSEHAT hanya ditampilkan sebagai roadmap.
