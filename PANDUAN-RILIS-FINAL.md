# Panduan Rilis Final Website Profil Dusun Pulesari

## 1. Sebelum upload

- Ekstrak ZIP final.
- Pastikan `index.html`, folder `assets/`, `css/`, dan `js/` berada langsung pada root folder proyek.
- Jangan hanya mengunggah file ZIP ke repository.
- Jangan mengunggah data penduduk atau dokumen internal.

## 2. GitHub Pages

1. Buat repository GitHub untuk situs Pulesari.
2. Unggah seluruh isi folder hasil ekstraksi ke root repository.
3. Buka **Settings → Pages**.
4. Pilih publikasi dari branch utama (umumnya `main`) dan folder `/(root)`.
5. Simpan pengaturan dan tunggu GitHub Pages menerbitkan situs.
6. Buka URL publik yang diberikan GitHub. Uji `index.html` dan seluruh 13 tautan halaman lainnya.

Contoh bentuk URL:

- User/organization site: `https://USERNAME.github.io/`
- Project site: `https://USERNAME.github.io/NAMA-REPOSITORY/`

Alamat contoh tersebut bukan URL situs Pulesari yang sudah aktif. Gunakan URL persis yang ditampilkan pada pengaturan GitHub Pages.

## 3. Pengujian sebelum Google Sites

- Buka website pada desktop, tablet, dan ponsel.
- Uji sidebar, menu mobile, pencarian lokal, tab, kalender, filter, tombol, dan modal.
- Uji apakah semua gambar tampil.
- Periksa apakah halaman masih menampilkan placeholder pada bagian data yang belum diberikan.
- Pastikan tidak ada identitas pribadi atau informasi administratif yang belum disetujui untuk publikasi.

## 4. Sematkan ke Google Sites

1. Buka Google Sites dan edit situs portal Pulesari.
2. Pilih halaman atau bagian yang akan menampilkan website.
3. Pilih **Sisipkan → Sematkan → URL**.
4. Masukkan URL GitHub Pages yang sudah aktif.
5. Atur lebar dan tinggi frame embed.
6. Periksa pratinjau desktop dan ponsel; sesuaikan tinggi frame agar konten tidak terpotong.

Jika tampilan di Google Sites tidak nyaman pada ponsel, tampilkan tautan **Buka Website Pulesari** menuju GitHub Pages secara jelas sebagai alternatif. Embed Google Sites memiliki bingkai dan tinggi tersendiri; uji pada halaman Sites yang benar-benar dipublikasikan.

## 5. Google Search — aktifkan hanya setelah konten siap

Saat ini halaman masih `noindex`. Jangan mengirim sitemap atau meminta pengindeksan sebelum data resmi, foto, dan konten publik telah diperiksa.

Setelah konten siap:

1. Pastikan URL GitHub Pages aktif melalui HTTPS.
2. Baca `SEO-LAUNCH-CHECKLIST.md`.
3. Jalankan generator SEO dari root proyek:

   ```bash
   python scripts/prepare-seo-launch.py --base-url https://USERNAME.github.io/NAMA-REPOSITORY/ --confirm-content-ready
   ```

   Ganti URL contoh dengan URL produksi yang sebenarnya. Untuk user/organization site, URL dasar biasanya berakhir pada `/` tanpa nama repository.

4. Periksa `sitemap.xml`, `robots.txt`, canonical URL, dan metadata sebelum commit.
5. Commit perubahan hasil generator dan tunggu GitHub Pages memperbarui situs.
6. Tambahkan properti URL-prefix di Google Search Console, verifikasi kepemilikan, kirim `sitemap.xml`, dan gunakan URL Inspection pada halaman utama serta halaman penting.

Pengindeksan dan posisi hasil pencarian ditentukan oleh Google; tidak ada jaminan waktu indeks atau peringkat tertentu.

## 6. Hal yang belum tersedia

ZIP ini tidak menyediakan hosting, database, autentikasi admin, email/form submission, atau penyimpanan berkas daring. Jika fitur tersebut diperlukan, siapkan backend dan layanan database terpisah sebelum mengumpulkan data warga.
