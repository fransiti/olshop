# README #

* Source code ini bebas untuk digunakan, namun harap mencantumkan nama pembuat pada footer olshop.

Aplikasi Olshop ini sendiri terbagi menjadi dua bagian, yaitu : bagian Frontend atau halaman untuk pengunjung dan juga bagian backend atau biasa disebut halaman untuk admin. Untuk halaman admin sendiri aplikasi ini menggunakan template Admin LTE versi Gentelella.

Aplikasi ini juga sudah menggunakan API yang disediakan oleh RajaOngkir sebagai penghitung ongkos kirimnya. Untuk itu jika sobat ingin menggunakan aplikasi ini, diharapkan sobat membuat akun RajaOngkir terlebih dahulu agar sobat mendapatkan API Key nya.

Selain sudah adanya fitur ongkir, aplikasi ini juga sudah menyediakan fitur-fitur lain, diantaranya :

* Adanya fitur Reset Password yang dikirim melalui E-mail yang memudahkan User untuk mereset password jika mereka lupa,
* Adanya fitur checkout yang sudah menggunakan API RajaOngkir untuk menghitung biaya total pembelian dan juga ongkos kirim
* Adanya fitur history transaksi
* dan masih banyak lagi

beberapa hal yang perlu dikonfigurasi sebelum menggukanan Olshop ini, diantaranya :
1. Database

pastikan sobat telah membuat dan menginport database yang ada pada folder source code ini, selanjutnya silahkan sobat buka file database.php yang ada pada folder application/config/ dan cari script berikut :

'database' => 'olshopku'

silahkan sobat ganti tulisan olshopku dengan nama database yang sobat buat.

2. API Key

konfigurasi yang kedua tentu saja untuk API Key RajaOngkir. Setelah sobat membuat akun di rajaongkir.com sobat akan mendapat sebuat kode acak, itu merupakan API Key milik sobat. Masukkan kode tersebut ke file Checkout.php yang ada di folder application/controllers/ kemudian cari script berikut :

"key : Your API KEY"

silahkan sobat ganti tulisan Your API KEY dengan kode API milik sobat.
kemudian sobat juga harus mengkonfigurasi file prov.php yang ada pada folder application/views/, silahkan sobat cari script seperti diatas dan ganti dengan kode API milik sobat.

3. Alamat Asal Pengiriman

untuk mengubah alamat asal pengiriman, silahkan sobat masuk ke menu checkout (klik icon keranjang) kemudian silahkan sobat pilih provinsi tempat tinggal sobat. jika sudah silahkan sobat lakukan inspect element untuk mengetahui id kota tempat tinggal sobat, kemudian silahkan sobat copy id tersebut. kemudian silahkan sobat buka file Checkout.php yang ada pada folder application/controllers/ dan cari script di bawah ini :

$asal = 305

ganti id 305 dengan id kota sobat semua.

4. Email

yang terakhir adalah mengkonfigurasi email, silahkan sobat buat sebuah akun gmail dan kemudian ubah script email@example yang ada pada file Lost_admin.php, Lost_user.php, dan juga Checkout.php yang ada pada folder application/controllers/. jika sudah pastikan juga pengaturan gmail nya, silahkan sobat masuk ke link : myaccount.google.com/security kemudian silahkan sobat cari Allow less secure apps jika statusnya masih OFF silahkan sobat ubah menjadi ON terlebih dahulu.

Copyright © 2017 OlShopKu. All Rights Reserved. - Develope By <a class="blue-text text-lighten-4" href="https://www.facebook.com/Jakdev28">Qomaruddin Rozzaq</a>

## TERIMA KASIH ### olshop
