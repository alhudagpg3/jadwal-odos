# Jadwal ODOS (PWA)

Aplikasi jadwal One Day One Juz untuk 8 atau 10 peserta. Berjalan di browser, bisa dipasang ke layar utama Android, dan bisa dipakai tanpa internet.

## Cara pasang di GitHub Pages
1. Buat repository baru di GitHub, misalnya `jadwal-odos` (Public).
2. Unggah semua file ini ke root repository: `index.html`, `style.css`, `app.js`, `data.js`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`.
3. Buka Settings > Pages. Pada Source pilih "Deploy from a branch", branch `main`, folder `/ (root)`, lalu Save.
4. Tunggu 1-2 menit. Alamatnya: `https://<username>.github.io/jadwal-odos/`.

## Pasang di Android
Buka alamat itu di Chrome, ketuk menu titik tiga, lalu "Instal aplikasi" (atau "Tambahkan ke layar utama").

## Catatan
- Nama peserta dan tanda sudah baca disimpan di HP masing-masing (localStorage), tidak dibagikan antar HP.
- Pembagian ayat dihitung dari tata letak Mushaf Madinah berdasarkan panjang teks (data di `data.js`).
- Ekspor: tombol "Ekspor Excel (CSV)" menghasilkan berkas yang bisa dibuka di Excel. "Cetak / PDF" memakai fitur cetak browser (pilih Simpan sebagai PDF).
- Setelah memperbarui file di GitHub, ubah `CACHE='odos-v1'` di `sw.js` menjadi `odos-v2` agar HP memuat versi baru.
