# Panduan Publikasi GitHub Pages dan Google Sites

## A. Unggah ke GitHub Pages

1. Buat repository GitHub baru atau gunakan repository yang memang disiapkan untuk website Pulesari.
2. Ekstrak ZIP ini di komputer.
3. Unggah seluruh isi folder ke root repository. Pastikan `index.html`, folder `assets`, `css`, dan `js` berada langsung di root repository.
4. Buka **Settings → Pages**.
5. Pada bagian Build and deployment, pilih deploy from a branch, pilih branch utama (misalnya `main`) dan folder `/(root)`, lalu simpan.
6. Tunggu proses publikasi selesai. Buka URL GitHub Pages yang ditampilkan dan uji halaman Beranda, Profil, serta seluruh menu.

## B. Sematkan di Google Sites

1. Buka Google Sites dan edit situs yang akan digunakan.
2. Pilih halaman tempat website akan ditampilkan.
3. Pilih **Sisipkan → Sematkan → URL**.
4. Masukkan URL GitHub Pages yang telah dipublikasikan.
5. Atur lebar embed selebar area konten dan tinggi sesuai kebutuhan.
6. Periksa kembali tampilan pratinjau desktop dan ponsel. Google Sites dapat memberikan tinggi bingkai embed tersendiri; sesuaikan tinggi komponen agar konten tidak terpotong.

## C. Catatan teknis

- Gunakan URL GitHub Pages sebagai alamat publik utama; Google Sites dapat menjadi portal yang menyematkannya.
- Jangan unggah data pribadi penduduk, NIK, dokumen internal, atau informasi sensitif ke repository publik.
- Formulir dan tombol prototipe pada versi ini belum mengirim data ke server.
- Fitur login, database, penyimpanan konten, dan pengelolaan dokumen memerlukan backend terpisah.
- Perbarui seluruh file di root repository saat menerapkan versi baru; jangan mengunggah ZIP sebagai satu file.


## SEO / Google Search setelah publikasi
1. Jangan kirim sitemap sebelum URL GitHub Pages dan konten resmi siap.
2. Setelah URL produksi diketahui dan placeholder telah diganti, jalankan script pada `scripts/prepare-seo-launch.py` sesuai `SEO-LAUNCH-CHECKLIST.md`.
3. Daftarkan properti URL-prefix GitHub Pages di Google Search Console, verifikasi kepemilikan, lalu kirim `sitemap.xml`.
4. Periksa halaman melalui URL Inspection. Pengindeksan tidak instan dan tidak dijamin.
5. Google Sites dapat digunakan sebagai portal/embeddable, tetapi URL GitHub Pages tetap menjadi URL kanonis untuk halaman HTML mandiri.

## Status rilis final (10 November 2026)

Paket final pra-publikasi berada pada versi 1.0.0. Seluruh 14 halaman utama dan 404 disertakan. Konten data dusun masih berupa placeholder; seluruh halaman publik tetap noindex sampai konten resmi diverifikasi. Sitemap produksi sengaja belum dibuat karena URL GitHub Pages belum diketahui. Laporan akhir ada di `docs/FINAL-QA-REPORT.json`.

Untuk langkah publikasi rinci dan SEO, lihat juga `PANDUAN-RILIS-FINAL.md` dan `SEO-LAUNCH-CHECKLIST.md`.
