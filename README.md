# Video Studio — Editor Video Sederhana

Versi awal editor video berbasis browser untuk menggabungkan gambar, klip, narasi, musik, dan subtitle menjadi MP4.

## Cara mencoba
1. Ekstrak ZIP ini.
2. Buka `index.html` melalui browser modern untuk melihat antarmuka. Untuk menjalankan mesin ekspor, lebih baik unggah file ke hosting HTTPS seperti GitHub Pages.
3. Saat pertama kali mengekspor, perangkat perlu terhubung ke internet agar mesin FFmpeg WebAssembly dimuat.
4. Tambahkan gambar/video, atur durasi gambar dan urutan, tambahkan audio atau subtitle, lalu pilih **Gabungkan dan ekspor MP4**.

## Publikasi GitHub Pages
1. Buat repositori GitHub baru.
2. Unggah `index.html`, `README.md`, `manifest.webmanifest`, dan `sw.js` ke folder utama repositori.
3. Buka **Settings → Pages**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu Save.
4. Buka alamat Pages yang ditampilkan GitHub.

## Catatan penting
- Ini versi awal; gunakan klip pendek untuk pengujian pertama.
- Pemrosesan dilakukan di browser, tetapi FFmpeg dimuat dari CDN sehingga perlu internet pada awal penggunaan.
- Perangkat HP dapat kehabisan memori untuk video besar; gunakan komputer untuk proyek panjang.
- Audio/codec tertentu atau subtitle tertanam dapat gagal bergantung pada browser dan build FFmpeg. Jika gagal, coba tanpa subtitle tertanam.
- Simpan salinan file asli. Aplikasi ini belum memiliki cloud save, akun, autosave proyek, efek kompleks, atau generator video AI.
