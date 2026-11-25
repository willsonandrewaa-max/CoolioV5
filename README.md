# Website Coolio — Panduan Edit

Buka `index.html` langsung di browser (double-click). Tidak perlu install apa pun.

## Struktur file
| File | Isi |
|---|---|
| `index.html` | Semua teks & susunan section (Hero, Masalah, Solusi, Produk, Target, Pasar, Keunggulan, Bisnis, Roadmap, Investasi, Kontak) |
| `style.css` | Tampilan. **Warna utama ada di bagian `:root` paling atas** |
| `script.js` | Botol 3D, efek semprot, animasi. **Teks label botol ada di `CONFIG` paling atas** |
| `assets/coolio-mockup-v2.webp` | Foto mockup produk (ganti file dengan nama sama untuk update foto) |
| `assets/problem-*-hd.jpg`, `ice.jpg`, `green-apple.jpg` | Foto section Problem & Solution |
| `assets/sdg-8-9.webp` | Badge SDG 8 & 9 |
| `assets/icon-*.png` | Ikon WhatsApp & Instagram di kontak |
| `assets/mascot-*.png` | Maskot Cools (hero, Problem, timeline produksi, Investment, kontak) |
| `assets/logo-word.webp` | Logo "Coolio" saja (navbar, hero, Why Coolio) |
| `assets/logo-full.webp` | Logo lengkap dengan tagline (bagian kontak) |
| `assets/logo-data.js` | Salinan logo untuk label botol 3D |

## Data dari proposal
Angka di section Market Opportunity, Business Model, dan Investment Opportunity diambil dari *02_Proposal_Indo_v02*. Kalau angka di proposal berubah, edit langsung teksnya di `index.html`.
- Grafik pendapatan: ubah `data-value` dan teks di tiap `<div class="col">`.
- Bar biaya per botol & anggaran: ubah `data-value` (persen panjang bar) dan teks nominalnya.

## Mode cerah / malam & mode HP
- Default **mode cerah**. Tombol bulan/matahari di navbar mengganti mode, dan pilihan pengunjung diingat di browser.
- Warna mode malam diatur di blok `[data-theme="dark"]` di akhir `style.css`. Botol 3D sengaja tetap putih di kedua mode.
- Di HP (layar ≤ 900px atau layar sentuh), website otomatis memakai **mode ringan**: botol 3D lebih sederhana, botol di section Product diganti foto, dan animasi dekoratif dimatikan. Pengaturannya ada di `MOBILE` (script.js) dan blok "MODE RINGAN UNTUK HP" (style.css).
- Semua gambar memakai format **.webp** agar cepat dimuat.

## Edit cepat lainnya
- **Keunggulan produk**: section `WHY COOLIO` di `index.html`.
- **Ganti warna**: palet brand ada di `:root` pada `style.css`: `--primary` #008EEB, `--secondary` #31B478, `--yellow` #FFF89F, `--accent` #FF009D (dipakai sedikit).
- **Ganti teks di label botol 3D**: ubah `CONFIG.label` di `script.js` (misal varian aroma baru).
- **Warna label botol 3D**: ubah `CONFIG.colors` di `script.js`.
- **Kecepatan putar botol**: `CONFIG.autoRotateSpeed` di `script.js`.
- **Menambah/menghapus section**: setiap section diberi komentar `<!-- ===== NAMA ===== -->` di `index.html`.

Data pasar bersumber dari The Report Cubes, *Indonesia Deodorants & Body Sprays Market Report and Forecast 2026–2034*.
