# Website Profil Dusun Pulesari — Rilis Final Pra-Publikasi

**Nama:** Website Profil Dusun Pulesari  
**Slogan:** Pulesari Migunani  
**Versi:** 1.0.0 — Final pra-publikasi  
**Status:** 14 halaman utama selesai dirakit; menunggu pengisian dan verifikasi data resmi.

## Isi website

| No. | Halaman | File |
|---:|---|---|
| 1 | Beranda | `index.html` |
| 2 | Profil Dusun | `profil-dusun.html` |
| 3 | Data Penduduk | `data-penduduk.html` |
| 4 | Produk Hukum Dusun | `produk-hukum-dusun.html` |
| 5 | Kelembagaan | `kelembagaan.html` |
| 6 | Program Dusun | `program-dusun.html` |
| 7 | Kegiatan & Agenda | `kegiatan-agenda.html` |
| 8 | Potensi Dusun | `potensi-dusun.html` |
| 9 | Peta Interaktif | `peta-interaktif.html` |
| 10 | Galeri & Dokumentasi | `galeri-dokumentasi.html` |
| 11 | Layanan Masyarakat | `layanan-masyarakat.html` |
| 12 | Pusat Informasi | `pusat-informasi.html` |
| 13 | Kontak Kami | `kontak.html` |
| 14 | Pengaturan | `pengaturan.html` |

## Menjalankan secara lokal

1. Ekstrak ZIP.
2. Buka terminal pada folder hasil ekstraksi.
3. Jalankan `python -m http.server 8000`.
4. Buka `http://localhost:8000` di browser.

Bisa juga membuka `index.html` langsung, tetapi server lokal lebih sesuai untuk menguji perilaku situs statis.

## Struktur proyek

- `index.html` dan 13 halaman HTML lain berada langsung di root.
- `css/` berisi gaya dasar, token desain, dan gaya khusus fase.
- `js/` berisi interaksi antarmuka sisi-klien.
- `assets/` berisi logo, banner, dan slot ilustrasi.
- `docs/` berisi inventaris halaman, design system, QA, dan aturan placeholder.
- `scripts/prepare-seo-launch.py` menyiapkan canonical URL, sitemap produksi, dan robots.txt setelah alamat publik diketahui serta konten siap.

## Status konten dan data

Data resmi Dusun Pulesari belum dimasukkan. Statistik, nama penduduk/pengurus, sejarah, visi-misi, batas wilayah, dokumen hukum, agenda, berita, foto kegiatan, kontak operasional, dan data potensi menggunakan placeholder atau status belum tersedia. Ilustrasi bukan dokumentasi faktual dusun.

Jangan mengisi atau menerbitkan NIK, nomor KK, tanggal lahir, alamat rumah, nomor telepon pribadi, maupun data keluarga melalui repository publik. Gunakan hanya informasi agregat yang telah diverifikasi dan disetujui untuk dipublikasikan.

## Batasan fungsional prototipe

Website ini merupakan situs statis. Beberapa interaksi sisi-klien seperti navigasi, tab, filter, kalender, preview galeri, preferensi tampilan lokal, dan dialog tersedia sesuai modul halaman. Namun, komponen berikut belum terhubung ke server:

- Login dan autentikasi admin.
- Database serta penyimpanan data penduduk/konten.
- Pengiriman formulir kontak, pengaduan, atau layanan.
- Unggah foto ke server dan manajemen file daring.
- Pengelolaan dokumen hukum melalui dashboard.
- Sinkronisasi pengaturan lintas perangkat.

Jangan menganggap tombol/formulir prototipe sebagai layanan administrasi aktif sebelum backend dan keamanan diimplementasikan.

## Status SEO pra-publikasi

- Setiap halaman memiliki title, meta description, dan metadata berbagi.
- Halaman masih menggunakan `noindex` sampai konten resmi diisi.
- `robots.txt` tersedia; sitemap produksi sengaja belum dibuat karena URL GitHub Pages belum diketahui.
- Jangan mengaktifkan indeks sebelum placeholder penting diganti dan semua informasi diperiksa.

Rujuk `SEO-LAUNCH-CHECKLIST.md` dan `PANDUAN-GITHUB-GOOGLE-SITES.md`. Script SEO produksi baru dijalankan setelah URL publik dipastikan dan pemilik proyek mengonfirmasi konten siap.

## Dokumen penting

- `PANDUAN-GITHUB-GOOGLE-SITES.md` — publikasi GitHub Pages dan embed Google Sites.
- `SEO-LAUNCH-CHECKLIST.md` — kesiapan Google Search.
- `ASSET-STATUS.md` — status logo, banner, dan ilustrasi.
- `docs/DATA-PLACEHOLDER-RULES.md` — aturan data kosong dan privasi.
- `docs/FINAL-QA-REPORT.json` — laporan pemeriksaan rilis.
- `FILE-MANIFEST.json` — daftar file dan checksum SHA-256.


## Responsive hotfix v1.1
Perbaikan sidebar laptop/tablet, hero image tablet/mobile, serta mobile portrait dan petunjuk ukuran embed Google Sites. Lihat `PANDUAN-RESPONSIVE-GOOGLE-SITES.md`.
