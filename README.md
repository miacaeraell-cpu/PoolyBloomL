# Pooly Bloom

Aplikasi statis berbasis HTML, CSS, dan JavaScript. Tidak memerlukan PHP, MySQL, Node.js, atau proses build. File `index.html` berada di root agar bisa langsung diterbitkan oleh GitHub Pages.

## Hosting di GitHub Pages

1. Buat repository baru di GitHub.
2. Unggah semua isi folder proyek ini ke root repository. Pastikan `index.html`, `.nojekyll`, dan folder `assets` berada di root yang sama.
3. Buka **Settings → Pages** pada repository.
4. Di bagian **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/(root)`, lalu tekan **Save**.
6. Setelah proses deploy selesai, buka alamat yang ditampilkan di halaman Pages. Untuk repository proyek, bentuk alamatnya `https://USERNAME.github.io/NAMA-REPOSITORY/`.

Panduan resmi: [Configure a publishing source for GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

Jika repository sudah dibuat, unggah/perbarui juga file terbaru dari folder `assets`. Halaman putih biasanya berarti `assets/app.js` belum ada di repository atau belum ikut ter-deploy. Perubahan di komputer tidak otomatis mengubah situs GitHub; perubahan harus diunggah/di-commit ke branch dan folder yang dipilih di Settings → Pages.

## Batasan penyimpanan

Data pesanan, katalog, transaksi, dan foto disimpan di `localStorage` browser. Setiap browser/perangkat mempunyai datanya sendiri; GitHub Pages tidak menyinkronkan data antarpengguna. Login bawaan di sisi browser bukan perlindungan keamanan karena kode aplikasi dapat dilihat publik. Jangan gunakan aplikasi ini untuk menyimpan data pelanggan atau keuangan yang rahasia. Buat backup JSON secara berkala melalui menu Pengaturan.

Login awal: **admin** / **Bloom@12345**. Ganti kata sandi melalui menu Pengaturan, tetapi ingat bahwa login ini hanya membatasi penggunaan kasual di browser tersebut.
