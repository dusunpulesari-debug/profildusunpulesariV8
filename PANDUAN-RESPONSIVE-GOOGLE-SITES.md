# Pulesari Mobile Portrait Fix v1.2

## Perubahan utama
- Beranda pada HP sekarang memakai artwork portrait 2:3, bukan banner landscape yang dipaksa masuk ke layar sempit.
- Teks sambutan berada di lapisan HTML agar terbaca dan dapat diubah tanpa mengedit gambar.
- Menu, kartu, panel, dan grid halaman ditumpuk dalam alur portrait pada lebar <= 760 px.
- Desktop tetap memakai banner horizontal dan sidebar penuh.
- Tablet menampilkan banner horizontal dengan rasio asli (tidak dipotong).
- Semua CSS, JavaScript, dan gambar hero untuk Beranda tertanam di masing-masing HTML.

## Penting tentang Google Sites
Google Sites menampilkan website dari GitHub Pages di dalam iframe. Tinggi iframe diatur terpisah oleh elemen embed Google Sites; CSS website tidak dapat memperbesar tinggi bingkai induknya. Jika tinggi embed hanya sekitar 250 px, pratinjau HP akan memperlihatkan bagian atas saja dan scrollbar internal.

Gunakan salah satu cara berikut:
1. Jika memakai **Sematkan menurut URL**, pilih elemen embed di editor Google Sites lalu tarik handle bawah sampai tinggi sekitar 2.500–3.000 px (sesuaikan lagi bila masih terpotong).
2. Jika memakai **Sematkan kode**, gunakan `GOOGLE-SITES-IFRAME-SNIPPET.html` yang sudah memakai tinggi 3.000 px. Jangan menempelkan seluruh HTML website ke Google Sites.

## Upload ke repository
1. Ekstrak ZIP ini.
2. Unggah seluruh isi hasil ekstraksi ke root repository `profildusunpulesariV7` (file `index.html` langsung di root).
3. Timpa file lama dengan nama yang sama, lalu commit ke branch `main`.
4. Tunggu GitHub Pages selesai deploy dan periksa URL V7.
5. Setelah GitHub Pages normal, perbarui/atur tinggi embed di Google Sites dan publikasikan ulang situs Google Sites.

## Data
Konten resmi, statistik, nama pengurus, agenda, dan dokumen masih placeholder sampai data terverifikasi tersedia.
