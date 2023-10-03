# Aplikasi Web "Opencart"

## Sekilas Tentang

Opencart adalah platform e-commerce berbasis web open-source yang dirancang untuk memungkinkan pemilik bisnis untuk membuat dan mengelola toko online mereka sendiri dengan mudah.
Platform ini memungkinkan user mengunggah produk dalam jumlah tak terbatas, menyiapkan metode pembayaran yang mudah, menambahkan beberapa toko, serta mengelola diskon dan afiliasi. Selain itu, fungsionalitas Opencart bisa ditingkatkan dengan modul PHP.

## Instalasi

### Prasyarat

- Unix, Linux atau Windows
- Apache Web Server 2.2+
- PHP 7.3+
- MySQL (gatau versi brp)
- RAM minimal 64 Mb+

### Langkah instalasi dalam CLI.
1. Pastikan seluruh paket sistem _up-to-date_ dan install ``XAMPP`` (Cross-platform Apache, PHP, dan MySQL). Selama instalasi XAMPP, pilih komponen ``Apache``, ``PHP``, dan ``MySQL`` untuk di install. https://www.apachefriends.org/index.html.
2. Install extension yang dibutuhkan dengan mengaktifkannya melalui panel kontrol XAMPP pilih ``config`` lalu buka ``PHP (php.ini)``
  - Cari line berikut di php.ini:
    ```
    ;extension=curl
    ;extension=gd
    ;extension=zip
    ```
  - Hapus ";" diawal line:
    ```
    extension=curl
    extension=gd
    extension=zip
    ```
4. Mulai layanan Apache dan MySQL dari panel kontrol XAMPP
5. Unduh Opencart ke dalam direktori kita.
```
git clone https://github.com/opencart/opencart.git
```
3. Ekstrak file yang telah diunduh ke dalam direktori yang kita inginkan.
4. Rename ``config-dist.php`` jadi ``config.php`` dan ``admin/config-dist.php`` jadi ``admin/config.php``
5. Buat database dengan nama ``opencart`` dan user untuk Opencart menggunakan ``phpMyAdmin``
6. Akses Opencart melalui browser dengan URL lokal ``http://localhost/opencart`` kemudian lakukan proses instalasi dengan mengikuti langkah-langkah instalasi yang ditampilkan termasuk konfigurasi database.
7. Hapus direktori instalasi untuk keamanan situs web.

## Konfigurasi (opsional)

Setting server tambahan yang diperlukan untuk meningkatkan fungsi dan kinerja aplikasi, misalnya:

- batas upload file
- batas memori
- dll

Plugin untuk fungsi tambahan

- login dengan Google/Facebook
- editor Markdown
- dll

## Maintenance (opsional)

Setting tambahan untuk maintenance secara periodik, misalnya:

- buat backup database tiap pekan
- hapus direktori sampah tiap hari
- dll

## Otomatisasi (opsional)

Skrip shell untuk otomatisasi instalasi, konfigurasi, dan maintenance.

## Cara Pemakaian

Cara pemaiakan CMS Opencart sangatlah mudah. Berikut langkah-langkahnya:

1. Saat kita membuka Opencart, maka kita akan masuk ke **Home Page** yang menampilkan produk-produk penjualan
   <img width="886" alt="image" src="https://github.com/lutfiahn24/Opencart/assets/93109340/f5000f6c-1985-4bc4-aa4c-cd2f352ced79">

2. Pada bagian atas terdapat menu berisi kategori dari produk yang dijual, sehingga kita dapat memilih kategori produk yang ingin ditampilkan
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/28f03b93-2ae7-493a-9511-71fc040f2d4b">

3. Kita juga dapat memilih mata uang yang kita pakai dengan menggunakan fitur **Currency** yang ada dipojok kiri atas
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/c39c75b8-44ca-4390-9760-4748a184794b">

4. Sebelum menggunakan Opencart lebih lanjut, kita perlu login terlebih dahulu dengan membuka tab **My Account** lalu pilih opsi **Login**
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/07445af2-5e6d-4631-a301-9dd40cbdd178">

5. Kita dapat menambahkan produk ke keranjang menggunakan fitur **Add to Cart**
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/943a0a5f-2dfe-4004-9ebc-af16fa06dbd6">

6. Untuk melihat daftar produk di keranjang, kita dapat menggunakan menu **Shopping Cart**. Disana kita bisa juga melihat estimasi biaya pengiriman dan penambahan code voucher
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/d024aa23-25bd-460f-9e1c-89268c9a8a88">

7. Menu **Checkout** digunakan saat kita akan melakukan pembelian dan pembayaran dengan mengisi data diri dan alamat serta memilih metode pengiriman dan metode pembayaran
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/298ad919-6949-48e3-aaeb-eb3e40dff1de">

8. Menu **Order History** dapat digunakan untuk melihat daftar pembayaran yang pernah dilakukan
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/cf4ee37b-6425-4918-b011-954a7ddc8e7f">

9. Menu **Wist List** digunakan untuk melihat daftar produk yang kita tambahkan sebagai wish list
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/26b7491b-78aa-4614-854f-100ad8c56189">

## Pembahasan

Opencart ditulis dalam bahasa pemrograman PHP yang support penggunaan MySQL. Kelebihan yang dimiliki oleh aplikasi Opencart yaitu:
    - Memiliki interface yang mudah digunakan, membuatnya cocok untuk digunakan oleh pemula.
    - Pengelolaan produk yang mudah dipahami dengan mengelompokkan produk sesuai kategori.
    - Beragamnya pilihan pembayaran membuat pengguna sangat fleksibel dalam memilih metode pembayaran yang diinginkan.
    - Mendukung dalam berbagai bahasa dan mata uang sehingga memungkinkan untuk menjangkau pasar global.

Kekurangan yang dimiliki Opencart yaitu:
    - Opencart tidak memiliki integrasi built-in yang kuat dengan berbagai fungsi manajemen bisnis lainnya.
    - Opencart kurang mampu dalam hal manajemen stok yang kompleks, manajemen persediaan, dan pemrosesan pesanan yang canggih.

Jika dibandingkan dengan aplikasi Odoo, Opencart memiliki beberapa kelebihan dan kekurangan:
    - Opencart dirancang khusus untuk toko online, Sedangkan Odoo mencakup berbagai aspek bisnis seperti akuntansi, CRM, produksi, persediaan, dan lainnya dalam satu platform terintegrasi.
    - Opencart memerlukan sumber daya server yang lebih sedikit dibandingkan dengan Odoo karena fokusnya yang lebih terbatas.
    - Versi Enterprise Odoo berbayar dan biayanya bisa lebih tinggi daripada biaya yang terkait dengan Opencart.

## Referensi

1. [Opencart](https://www.opencart.com)
