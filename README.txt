WIJANA MOJOAGUNG — FLIPBOOK V4

V4 memperbaiki dua masalah V2/V3:
1. State halaman sekarang eksplisit:
   cover -> spread 2-3 -> spread 4-5 -> ... -> spread 22-23 -> back cover 24.
2. Animasi tidak lagi mengubah current page dengan rumus yang dapat melompati
   halaman. Setiap aksi navigasi memiliki transisi dan target yang jelas.

Perbaikan rendering:
- PDF.js merender halaman ke canvas.
- Canvas dikonversi menjadi image data URL.
- Image asli disimpan dan di-clone untuk tampilan/animasi.
- Tidak menggunakan cloneNode() pada canvas yang sudah dilukis.

Menjalankan:
1. Buka folder di Visual Studio Code.
2. Pastikan Live Server terpasang.
3. Klik kanan index.html -> Open with Live Server.
4. Buka localhost yang diberikan.

Catatan:
V4 masih prototype visual. Setelah fungsi dasar stabil, tahap berikutnya adalah
menambahkan drag/swipe page-turn yang lebih realistis, shadow lipatan, klik area
halaman, dan optimasi agar tidak merender semua halaman sekaligus.
