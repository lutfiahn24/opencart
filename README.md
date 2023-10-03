# Aplikasi Web "Opencart"

## Sekilas Tentang

Opencart adalah platform e-commerce berbasis web open-source yang dirancang untuk memungkinkan pemilik bisnis untuk membuat dan mengelola toko online mereka sendiri dengan mudah.
Platform ini memungkinkan user mengunggah produk dalam jumlah tak terbatas, menyiapkan metode pembayaran yang mudah, menambahkan beberapa toko, serta mengelola diskon dan afiliasi. Selain itu, fungsionalitas Opencart bisa ditingkatkan dengan modul PHP.

## Instalasi

### Prasyarat

- Unix, Linux atau Windows
- Apache Web Server 2.2+
- PHP 8.0+
- MySQL
- RAM minimal 64 Mb+

### Langkah instalasi dalam CLI.

1. Pastikan seluruh paket sistem _up-to-date_ dan install `XAMPP` (Cross-platform Apache, PHP, dan MySQL). Selama instalasi XAMPP, pilih komponen `Apache`, `PHP`, dan `MySQL` untuk di install. https://www.apachefriends.org/index.html.
2. Install extension yang dibutuhkan dengan mengaktifkannya melalui panel kontrol XAMPP pilih `config` lalu buka `PHP (php.ini)`

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

3. Mulai layanan Apache dan MySQL dari panel kontrol XAMPP
4. Unduh Opencart ke dalam direktori kita.

```
git clone https://github.com/opencart/opencart.git
```

5. Ekstrak file yang telah diunduh ke dalam direktori yang kita inginkan.
6. Rename `config-dist.php` jadi `config.php` dan `admin/config-dist.php` jadi `admin/config.php`
7. Buat database dengan nama `opencart` dan user untuk Opencart menggunakan `phpMyAdmin`
8. Akses Opencart melalui browser dengan URL lokal `http://localhost/opencart` kemudian lakukan proses instalasi dengan mengikuti langkah-langkah instalasi yang ditampilkan

- Setujui persyaratan yang berlaku
  ![WhatsApp Image 2023-10-03 at 11 45 53_88737a42](https://github.com/lutfiahn24/opencart/assets/93109340/b89cea78-01b2-4554-b06d-b12ca2499b51)
- Pemeriksaan server, lengkapi konfigurasi PHP dan kelengkapan extension
  ![WhatsApp Image 2023-10-03 at 10 50 56_e277664a](https://github.com/lutfiahn24/opencart/assets/93109340/ebb92d52-884e-4dd3-9af4-9496bbd96222)
- Konfigurasi database
  ![WhatsApp Image 2023-10-03 at 10 53 47_a1ee759c](https://github.com/lutfiahn24/opencart/assets/93109340/8e90fde1-be3b-4a0f-8d03-1d52aa6a2950)

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

## Otomatisasi

Opencart dihosting menggunakan layanan _web-hosting_ dan domain dari https://www.rumahweb.com/. Tujuan dari hosting adalah agar Opencart dapat diakses secara _online_. Berikut langkah-langkah hosting Opencart :
1. Sewa layanan hosting dan domain dari rumahweb. Domain yang digunakan adalah opencartonline.my.id.
   
2. Login ke cPanel dari akun rumahweb.
   <img width="886" alt="Screenshot (1289)" src="https://github.com/lutfiahn24/opencart/assets/146713686/c4e1d585-f425-4446-8ab9-7be7b36cdd9c">

3. Pada cPanel pilih file manager di menu files.
   <img width="886" alt="Screenshot (1290)" src="https://github.com/lutfiahn24/opencart/assets/146713686/82808190-a9bb-4f92-853b-61c1e594fc92">

4. Upload folder zip opencart-master yang telah diunduh dan letakkan di dalam folder public_html. Kemudian ekstrak file zip
   opencart-master.

   <img width="886" alt="Screenshot (1292)" src="https://github.com/lutfiahn24/opencart/assets/146713686/de3b8a4d-b277-47c5-a86e-351ec0bf0fa9">

6. Buka folder upload pada folder opencart-master dan hapus file index.php


## Cara Pemakaian

Cara pemaiakan CMS Opencart sangatlah mudah. Berikut langkah-langkahnya:

1. Login sebagai admin.
   <img width="886" alt="Login" src="https://github.com/lutfiahn24/opencart/assets/118100945/1b3ee030-4df5-4fbc-a24b-d9c21b4b9e22">

2. Setelah login akan masuk ke page **Dashboard**
   <img width="886" alt="Dashboard" src="https://github.com/lutfiahn24/opencart/assets/118100945/dfd14126-e299-4e90-b24f-be138b5ece36">

3. Navbar disamping menyediakan beberapa fitur yang dapat digunakan oleh admin untuk mempermudah admin.
   Beberapa contoh fitur yang akan kami tampilkan adalah sebagai berikut:
   Untuk menambahkan produk baru dapat dilakukan dengan menuju **Catalog** yang ada pada Navbar disamping lalu **Products**.
   Setelah itu dipojok kanan atas terdapat icon **+** lalu isi detail dari produk yang akan ditambahkan.
   <img width="886" alt="Screenshot 2023-10-03 at 11 50 47" src="https://github.com/lutfiahn24/opencart/assets/118100945/bbf80d85-5103-4c8d-a4d0-2053ac34ba52">

4. Untuk melihat daftar **Order** terdapat pada menu **Sales**.
   <img width="886" alt="Order" src="https://github.com/lutfiahn24/opencart/assets/118100945/d19d0e79-8eb8-49ed-8ec4-f3ae10999b88">

5. Untuk melihat berapa banyak Customer yang melakukan registrasi terdapat pada menu **Customers**.
   <img width="886" alt="Customer" src="https://github.com/lutfiahn24/opencart/assets/118100945/b7e809c8-c5f1-415f-bb27-f14ddb5a9f35">

Adapun cara pemakaian CMS OpenCart sebagai User.

1. Melakukan registrasi pada menu **Register Account**.
   <img width="886" alt="Register " src="https://github.com/lutfiahn24/opencart/assets/118100945/70bc891d-43af-46e0-9d75-698e5ed9670b">

2. Saat kita membuka Opencart, maka kita akan masuk ke **Home Page** yang menampilkan produk-produk penjualan
   <img width="886" alt="image" src="https://github.com/lutfiahn24/Opencart/assets/93109340/f5000f6c-1985-4bc4-aa4c-cd2f352ced79">

3. Pada bagian atas terdapat menu berisi kategori dari produk yang dijual, sehingga kita dapat memilih kategori produk yang ingin ditampilkan
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/28f03b93-2ae7-493a-9511-71fc040f2d4b">

4. Kita juga dapat memilih mata uang yang kita pakai dengan menggunakan fitur **Currency** yang ada dipojok kiri atas
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/c39c75b8-44ca-4390-9760-4748a184794b">

5. Sebelum menggunakan Opencart lebih lanjut, kita perlu login terlebih dahulu dengan membuka tab **My Account** lalu pilih opsi **Login**
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/07445af2-5e6d-4631-a301-9dd40cbdd178">

6. Kita dapat menambahkan produk ke keranjang menggunakan fitur **Add to Cart**
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/943a0a5f-2dfe-4004-9ebc-af16fa06dbd6">

7. Untuk melihat daftar produk di keranjang, kita dapat menggunakan menu **Shopping Cart**. Disana kita bisa juga melihat estimasi biaya pengiriman dan penambahan code voucher
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/d024aa23-25bd-460f-9e1c-89268c9a8a88">

8. Menu **Checkout** digunakan saat kita akan melakukan pembelian dan pembayaran dengan mengisi data diri dan alamat serta memilih metode pengiriman dan metode pembayaran
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/298ad919-6949-48e3-aaeb-eb3e40dff1de">

9. Menu **Order History** dapat digunakan untuk melihat daftar pembayaran yang pernah dilakukan
   <img width="886" alt="image" src="https://github.com/lutfiahn24/OpenCart/assets/93109340/cf4ee37b-6425-4918-b011-954a7ddc8e7f">

10. Menu **Wist List** digunakan untuk melihat daftar produk yang kita tambahkan sebagai wish list
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
2. [Cara Install Opencart: Panduan untuk Pemula](https://www.hostinger.co.id/tutorial/cara-install-opencart#:~:text=OpenCart%20adalah%20sistem%20manajemen%20konten,usaha%20kecil%20maupun%20perusahaan%20besar.)
