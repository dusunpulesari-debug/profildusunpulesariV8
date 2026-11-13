# Checklist SEO sebelum peluncuran Google Search

## A. Kesiapan konten

- [ ] Isi dan verifikasi sejarah, identitas, lokasi, visi-misi, serta batas wilayah.
- [ ] Isi statistik hanya dari rekap agregat yang telah diverifikasi.
- [ ] Pastikan tidak ada NIK, nomor KK, tanggal lahir, alamat rumah, atau data pribadi sensitif di halaman publik.
- [ ] Verifikasi nama lembaga, pengurus, program, agenda, potensi, layanan, dan persyaratan.
- [ ] Ganti ilustrasi sementara dengan logo/foto resmi jika sudah tersedia; jangan menandai ilustrasi sebagai foto dokumentasi asli.
- [ ] Hapus placeholder yang tidak relevan dan pastikan setiap halaman memiliki konten unik yang bermanfaat.
- [ ] Minta persetujuan pengelola dusun untuk konten yang akan dipublikasikan.

## B. Kesiapan teknis

- [ ] Unggah semua isi ZIP ke root repository GitHub Pages; `index.html` harus berada di root.
- [ ] Pastikan URL GitHub Pages aktif melalui HTTPS.
- [ ] Uji semua 14 halaman di desktop, tablet, dan ponsel.
- [ ] Periksa navigasi, gambar, tautan, formulir, dan fitur prototipe.
- [ ] Catat URL publik yang benar, termasuk nama repository jika memakai project site.

## C. Aktifkan SEO produksi

**Jangan lakukan sebelum A dan B selesai.** Saat ini halaman publik masih `noindex` dan sitemap produksi belum tersedia.

Jalankan dari root proyek setelah URL produksi diketahui dan konten disetujui:

```bash
python scripts/prepare-seo-launch.py --base-url https://USERNAME.github.io/NAMA-REPOSITORY/ --confirm-content-ready
```

Ganti URL contoh dengan alamat sebenarnya. Script akan mengaktifkan indexing pada 13 halaman publik, menambahkan canonical dan metadata URL, lalu membuat `sitemap.xml` serta memperbarui `robots.txt`. Halaman Pengaturan dan 404 tetap `noindex,nofollow`.

Setelah menjalankan script:
- [ ] Periksa isi canonical setiap halaman.
- [ ] Periksa `sitemap.xml` dan `robots.txt`.
- [ ] Commit hasil perubahan ke GitHub.
- [ ] Buat properti URL-prefix di Google Search Console dan verifikasi kepemilikan.
- [ ] Kirim sitemap produksi.
- [ ] Gunakan URL Inspection untuk halaman utama dan halaman penting.
- [ ] Pantau laporan pengindeksan dan perbaiki masalah yang dilaporkan.

Google tidak menjamin setiap halaman diindeks atau memperoleh posisi tertentu. Hasil pencarian membutuhkan waktu dan bergantung pada evaluasi Google.
