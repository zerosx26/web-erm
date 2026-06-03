# WEB ERM

Static landing page publik untuk produk **ERM Offline**.

## Struktur

- `index.html` - landing page utama.
- `styles.css` - styling responsif clean medical SaaS.
- `script.js` - interaksi kecil untuk menu mobile, smooth scroll, dan galeri screenshot.
- `assets/screenshots/` - visual screenshot-style sementara. Ganti dengan screenshot asli aplikasi dari preview/build ERM Offline saat tersedia.
- `sales/` - materi marketing awal: penawaran, checklist demo, script WhatsApp, dan tracker lead CSV.

## Aktivasi WhatsApp CTA

Edit `script.js`, lalu isi:

```js
const WHATSAPP_NUMBER = "628xxxxxxxxxx";
```

Gunakan format internasional tanpa `+`, spasi, atau tanda baca.

## Materi Sales

- `sales/penawaran-erm-offline.md` untuk dikirim setelah calon pembeli tertarik.
- `sales/demo-15-menit-checklist.md` untuk alur demo.
- `sales/script-whatsapp.md` untuk chat awal dan follow-up.
- `sales/lead-tracker.csv` untuk mencatat 10-20 calon pengguna pertama.

## Deploy GitHub Pages

1. Buat repository publik `zerosx26/web-erm`.
2. Push isi folder ini ke branch `main`.
3. Buka **Settings > Pages**.
4. Pilih **Deploy from a branch**, branch `main`, folder `/root`.
5. URL publik yang diharapkan: `https://zerosx26.github.io/web-erm/`.

## Catatan

- CTA WhatsApp masih placeholder dan perlu diganti saat nomor sales final tersedia.
- Jangan masukkan source Flutter, license generator, secret, database, atau dokumen internal ke repo ini.
- Klaim cloud, Android companion, dan SATUSEHAT hanya ditampilkan sebagai roadmap.
