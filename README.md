
## Overview

Artikel ini akan membahas beberapa hal yang akan membantu kamu mencoba Spark AR untuk pertama kalinya, beberapa hal yang akan dicakup dalam artikel ini adalah

* Persiapan dan cara menginstall Spark AR
* Membuat filter sederhana berupa Flash Card dengan fitur Gallery Texture
* Testing dan langkah-langkah untuk mempublish filter yang telah kita buat 

Diharapkan setelah mengikuti artikel ini kamu sudah bisa membuat filter mu sendiri yang dapat berfungsi dengan baik dan berhasil merilisnya untuk digunakan oleh masyarakat umum.


## Menginstall Spark AR

Spark AR adalah software yang akan membantu kita untuk blablabla

### Persyaratan
Untuk menginstall Spark AR ada beberapa hal yang perlu kita persiapkan, diantaranya adalah

#### Hardware
Spark AR membutuhkan PC dengan spesifikasi minimum seperti berikut
* Sistem Operasi : Minimum Windows 10 (64 bit) atau MacOS 10.14+
* RAM minimum 4GB
* GPU minimal 
* CPU minimal Intel Core i3 2.5Ghz, or AMD Bulldozer/Jaguar/Puma/Zen with SSE4.1



#### Akun
Untuk menggunakan Spark AR dan mempublikasikan Filter yang akan kita buat, dibutuhkan beberapa akun yaitu :
* Akun Facebook, untuk login dan menggunakan Spark AR serta mengorganisir project yang akan kita publish.
* Akun Instagram yang terkoneksi dengan akun Facebook tadi, untuk testing dan publishing Filter yang kita buat.

Apabila seluruh persyaratan telah terpenuhi sekarang kita bisa mulai install Spark AR dengan mengunduh versi terbarunya di

https://sparkar.facebook.com/ar-studio/learn/downloads/#spark-ar-studio

Saat artikel ini dibuat, versi terbaru yang digunakan adalah v98.

### Login Facebook
Hal yang akan muncul saat kita pertama kali membuka Spark AR adalah popup login akun Facebook, isilah dengan data akunmu dan kemudian kamu dapat menggunakan Spark AR.

![login](tutorial_images/00_login.PNG)

Untuk Logout Spark AR dari akun yang digunakan saat ini, bisa dilakukan dengan cara : klik **File** lalu pilih **Logout**

## Membuat Project Baru

Tampilan awal dari SparkAR adalah ///. Kamu bisa membuka dan mempelajari beberapa template yang disediakan, dan terdapat beberapa tutorial yang bisa kamu ikuti.

![homepage](tutorial_images/01_homepage.PNG)

### Membuka Blank Project

Untuk saat ini kita akan memulai dengan membuat project baru dari awal.

Klik **Create New** > **New Project**

Akan ditampilkan popup tipe project yang bisa kamu buat. Karena saat ini kita akan belajar dari awal, maka pilihlah **Blank Project**

![project baru](tutorial_images/02_new_project.gif)


### Tampilan utama Spark AR
Spark AR akan membuka sebuah window baru yang akan menjadi workarea kita. Jika diperhatikan, workarea kita terbagi menjadi beberapa area utama.

![mainview](tutorial_images/03_Main_View.PNG)

- A adalah panel Scene. Scene berguna untuk mengatur hirearki objek-objek yang akan kita gunakan. Secara default sudah disiapkan Ambient Light dan Directional Light. Untuk project ini akan kita abaikan saja kedua object light tersebut.
- B adalah panel Assets. Panel Assets akan kita gunakan untuk mengorganisir file yang kita gunakan pada project, seperti Image dan Material
- C adalah panel View. Pada bagian tengah akan menjadi work area utama dimana kita bisa melihat dan mengedit secara langsung posisi dan ukuran objek-objek pada projek kita
- D adalah panel Properties. Pada sisi kanan tersedia panel Properties yang bisa digunakan untuk mengatur setting dari object yang kita gunakan


