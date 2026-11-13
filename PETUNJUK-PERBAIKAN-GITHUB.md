# Perbaikan tampilan GitHub Pages Pulesari

## Diagnosis
Website pada URL `https://dusunpulesari-debug.github.io/profildusunpulesariV7/` menampilkan HTML tanpa gaya karena berkas pendukung yang dipanggil oleh HTML tidak tersedia pada repository GitHub yang saat ini terbit.

Contoh file yang harus ada:
- `css/app.css`
- `css/phase10.css`
- `css/phase5.css`
- `css/phase11.css`
- `assets/logo-pulesari.webp`
- `assets/beranda-hero.webp`
- `js/app.js`

Pemeriksaan URL raw pada repository saat diagnosis mengembalikan 404 untuk `css/app.css`, `assets/beranda-hero.webp`, dan `js/app.js`.

## Struktur root repository yang benar
Pastikan setelah upload, repository memiliki struktur berikut. Folder harus berada sejajar dengan `index.html`, bukan berada di dalam folder ZIP atau folder proyek tambahan.

```
repository/
├── index.html
├── profil-dusun.html
├── data-penduduk.html
├── produk-hukum-dusun.html
├── kelembagaan.html
├── program-dusun.html
├── kegiatan-agenda.html
├── potensi-dusun.html
├── peta-interaktif.html
├── galeri-dokumentasi.html
├── layanan-masyarakat.html
├── pusat-informasi.html
├── kontak.html
├── pengaturan.html
├── 404.html
├── css/
├── js/
├── assets/
├── docs/
├── scripts/
├── robots.txt
└── .nojekyll
```

## Cara memperbaiki
1. Unduh ZIP perbaikan ini dan ekstrak di komputer.
2. Buka repository `dusunpulesari-debug/profildusunpulesariV7`.
3. Unggah ulang **seluruh isi hasil ekstrak**, termasuk folder `css`, `js`, `assets`, `docs`, dan `scripts` beserta file HTML di root.
4. Jangan hanya mengunggah file HTML. Jangan menaruh seluruh isi di dalam satu folder tambahan seperti `PULESARI-WEBSITE-PROFIL-FINAL/`.
5. Commit perubahan ke branch `main`.
6. Tunggu GitHub Pages selesai melakukan deployment.

Cara yang paling aman adalah menggunakan GitHub Desktop: clone repository, salin seluruh isi hasil ekstrak ke folder repository lokal (pilih replace/overwrite bila diminta), commit, lalu push ke GitHub.

## Pemeriksaan setelah upload
Buka URL berikut. Masing-masing harus terbuka dan tidak menghasilkan 404:
- `https://dusunpulesari-debug.github.io/profildusunpulesariV7/css/app.css`
- `https://dusunpulesari-debug.github.io/profildusunpulesariV7/assets/beranda-hero.webp`
- `https://dusunpulesari-debug.github.io/profildusunpulesariV7/js/app.js`

Jika ketiganya berhasil, buka kembali halaman utama dengan hard refresh (`Ctrl+Shift+R`). Setelah itu, sematkan URL utama GitHub Pages di Google Sites melalui **Sisipkan → Sematkan → Menurut URL**. Jangan tempel kode HTML ke kotak embed.

## Catatan
Paket ini adalah website statis. Fitur yang memerlukan penyimpanan server, akun admin, pengiriman formulir, atau database tetap membutuhkan backend terpisah. Isi data resmi dusun masih berupa placeholder sesuai arahan pemilik proyek.
