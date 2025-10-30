# lab6web.
# Richie Pranata 
# TI.24.A.5
# 312410451

### Penjelasan
Kode HTML gabungan ini mengambil elemen-elemen layout utama dari kedua file, portofolio.html (profil dan tata letak modern) dan index.html (fungsionalitas JavaScript dan demo layout dasar), dan menyatukannya dalam satu halaman menggunakan Bootstrap 5.

### 1. Struktur Penggabungan dan Halaman
Struktur halaman ini dibagi menjadi beberapa bagian utama agar mudah dinavigasi dan dikelola.

HEAD Section	Gabungan Keduanya	Berisi semua metadata, satu tautan Bootstrap CSS, CSS kustom yang digabungkan, dan semua definisi fungsi JavaScript dari index.html.

BODY OnLoad	index.html	Mengandung onload="pesanOnLoad()" yang menampilkan pesan alert saat halaman selesai dimuat.

Navbar	portofolio.html	Menu navigasi sticky di bagian atas, kini memiliki tautan ke semua bagian baru (#about, #portfolio, #js-demo, #layout-demo).

Hello World!	index.html	Bagian ini adalah hasil eksekusi dari document.write(), diletakkan di bawah Navbar
Tentang Saya (#about)	portofolio.html	Menampilkan profil pribadi.

Portfolio (#portfolio)	portofolio.html	Menampilkan daftar proyek (card view).

Demo JavaScript (#js-demo)	index.html	Menjadi pusat demonstrasi semua fungsionalitas JavaScript interaktif.

Demo Layout Utama (#layout-demo)	index.html	Menampilkan struktur main (8 kolom) dan sidebar (4 kolom) dengan contoh featurette dan widget.

Footer	portofolio.html	Bagian bawah halaman untuk informasi hak cipta.

### 2. Fungsi Utama Fungsionalitas JavaScript
Semua fungsi JavaScript didefinisikan dalam tag <script> di bagian <head> dan dipanggil menggunakan event handler seperti onclick atau onsubmit di elemen-elemen HTML pada bagian #js-demo.

pesanOnLoad()	Menampilkan kotak dialog alert saat halaman web selesai dimuat (Event onload).	Atribut onload pada tag <body>.

document.write()	Menulis konten HTML ("Hello World!") langsung ke dokumen.	<script> inline di dalam <body>.

ubahwarnaLB(warna)	Mengubah warna latar belakang (backgroundColor) seluruh dokumen HTML.	onclick pada tombol "LB Hijau" dan "Reset Warna".

ubahwarnaLD(warna)	Mengubah warna teks (color) seluruh dokumen HTML.	onclick pada tombol "Teks Kuning" dan "Reset Warna".

testGenapGanjil()	Memvalidasi input angka dan menentukan apakah bilangan tersebut genap atau ganjil.	onclick pada tombol "TEBAK".

validateForm()	Memeriksa apakah input Nama dan Usia pada form telah diisi dan Usia berupa angka. Menampilkan alert jika validasi gagal.	onsubmit pada tag <form name="myForm">.

runPromptAndIfElse()	Menggunakan fungsi prompt() untuk meminta input pengguna, lalu menampilkan hasil keputusan If-Else (lulus/tidak lulus).	onclick pada tombol "Jalankan Prompt & If-Else".

testSwitch()	Menggunakan fungsi prompt() untuk input, lalu menggunakan struktur Switch Case untuk menentukan output berdasarkan nilai yang dimasukkan (1-5).	onclick pada tombol "Jalankan Switch Case".

hitung(ele)	Menggunakan DOM Manipulation untuk menghitung total harga makanan berdasarkan checkbox yang dicentang.	onclick pada setiap checkbox di bagian "Hitung Total Menu Makanan

### 3. Fungsi Komponen Layout HTMLKomponen Layout
NAVBAR(Sticky)Menyediakan navigasi utama yang tetap terlihat saat pengguna menggulir halaman ke bawah, memastikan akses mudah ke semua bagian (Tentang Saya, Portfolio, JS Demo, Layout Demo).

#about & #portfolioBagian utama untuk konten Portofolio: menampilkan informasi pribadi (dengan gambar dan deskripsi) dan karya atau proyek-proyek dalam format kartu (Card).

#main (Kolom 8)Bagian konten utama di Demo Layout. Berisi tata letak 3 kolom untuk Heading dan dua artikel panjang (Featurette) dengan gambar yang di-float.

#sidebar (Kolom 4)Bagian samping di Demo Layout. Berisi widget tambahan, seperti daftar tautan dan blok teks informasi, memisahkan konten pendukung dari konten utama.<footer>Menutup halaman, berisi informasi hak cipta.

Bootstrap CDNMenyediakan kerangka kerja (CSS dan JavaScript) agar tata letak dan komponen (seperti Navbar, Card, Form, Button, Grid System) menjadi responsif dan bergaya modern.
