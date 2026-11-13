# Website Profil Dusun Pulesari — Paket Single HTML

Versi ini dibuat untuk mengurangi risiko file CSS, JavaScript, dan aset gambar tidak ikut terbaca saat diunggah ke GitHub Pages atau disematkan di Google Sites.

## Struktur

Setiap halaman HTML sudah membawa CSS, JavaScript, logo, dan gambar lokal yang dipakai oleh halaman itu secara langsung di dalam file HTML (inline/data URI). Karena itu folder `css/`, `js/`, dan `assets/` tidak diperlukan untuk menjalankan halaman.

File HTML utama berada langsung di root repository. Upload isi ZIP ini ke root repository GitHub, bukan ke dalam folder bertingkat.

## File halaman

- `index.html` — Beranda
- `profil-dusun.html`
- `data-penduduk.html`
- `produk-hukum-dusun.html`
- `kelembagaan.html`
- `program-dusun.html`
- `kegiatan-agenda.html`
- `potensi-dusun.html`
- `peta-interaktif.html`
- `galeri-dokumentasi.html`
- `layanan-masyarakat.html`
- `pusat-informasi.html`
- `kontak.html`
- `pengaturan.html`
- `404.html`

## Upload GitHub Pages

1. Ekstrak ZIP.
2. Masuk ke repository `profildusunpulesariV7`.
3. Hapus atau timpa file HTML lama dan unggah semua isi ZIP ke root repository.
4. Pastikan `index.html` terlihat di halaman utama repository bersama folder `docs/`, `scripts/`, serta file `robots.txt` dan `.nojekyll`.
5. Commit ke branch yang dipakai GitHub Pages (misalnya `main`).
6. Setelah deployment selesai, buka URL GitHub Pages.
7. Setelah situs langsung terbuka dengan benar, gunakan URL tersebut pada Google Sites melalui Sisipkan → Sematkan → Menurut URL.

## Catatan

- Font Google dapat memerlukan koneksi internet; jika gagal, font fallback akan digunakan.
- Peta dan tautan Google Maps memerlukan internet.
- Website masih menggunakan placeholder; data resmi belum diisi.
- Formulir, penyimpanan data, autentikasi admin, dan database membutuhkan backend.
- SEO tetap `noindex` sampai data resmi dan URL final siap dipublikasikan.
