
# Overview

Artikel ini akan membahas beberapa hal yang akan membantu kamu mencoba Spark AR untuk pertama kalinya, beberapa hal yang akan dicakup dalam artikel ini adalah

* Persiapan dan cara menginstall Spark AR
* Membuat filter sederhana berupa Flash Card dengan fitur Gallery Texture
* Testing dan langkah-langkah untuk mempublish filter yang telah kita buat 

Diharapkan setelah mengikuti artikel ini kamu sudah bisa membuat filter mu sendiri yang dapat berfungsi dengan baik dan berhasil merilisnya untuk digunakan oleh masyarakat umum.


# Menginstall Spark AR

Spark AR adalah software yang akan membantu kita untuk blablabla

## Persyaratan
Untuk menginstall Spark AR ada beberapa hal yang perlu kita persiapkan, diantaranya adalah

### Hardware
Spark AR membutuhkan PC dengan spesifikasi minimum seperti berikut
* Sistem Operasi : Minimum Windows 10 (64 bit) atau MacOS 10.14+
* RAM minimum 4GB
* GPU minimal 
* CPU minimal Intel Core i3 2.5Ghz, or AMD Bulldozer/Jaguar/Puma/Zen with SSE4.1



### Akun
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

# Membuat Project Baru

Tampilan awal dari SparkAR adalah ///. Kamu bisa membuka dan mempelajari beberapa template yang disediakan, dan terdapat beberapa tutorial yang bisa kamu ikuti.

![homepage](tutorial_images/01_homepage.PNG)

## Membuka Blank Project

Untuk saat ini kita akan memulai dengan membuat project baru dari awal.

Klik **Create New** > **New Project**

Akan ditampilkan popup tipe project yang bisa kamu buat. Karena saat ini kita akan belajar dari awal, maka pilihlah **Blank Project**

![project baru](tutorial_images/02_new_project.gif)


## Tampilan utama Spark AR
Spark AR akan membuka sebuah window baru yang akan menjadi workarea kita. Jika diperhatikan, workarea kita terbagi menjadi beberapa area utama.

![mainview](tutorial_images/03_Main_View.PNG)

- A adalah panel Scene. Scene berguna untuk mengatur hirearki objek-objek yang akan kita gunakan. Secara default sudah disiapkan Ambient Light dan Directional Light. Untuk project ini akan kita abaikan saja kedua object light tersebut.
- B adalah panel Assets. Panel Assets akan kita gunakan untuk mengorganisir file yang kita gunakan pada project, seperti Image dan Material
- C adalah panel View. Pada bagian tengah akan menjadi work area utama dimana kita bisa melihat dan mengedit secara langsung posisi dan ukuran objek-objek pada projek kita
- D adalah panel Properties. Pada sisi kanan tersedia panel Properties yang bisa digunakan untuk mengatur setting dari object yang kita gunakan


## Menambahkan Face Tracker
Mendeteksi wajah adalah hal utama yang kita butuhkan untuk membuat filter ini, dengan menggunakan Spark AR fitur ini sangat mudah kita buat karena Spark AR telah menyediakan beberapa jenis Tracker diantaranya Face Tracker

Untuk menggunakan Face Tracker sangatlah mudah, pada panel **Scene** klik tombol **Add Object** yang berada di sisi kanan bawah lalu pilih **Face Tracker** kemudian klik **Insert**

![add face tracker](tutorial_images/04_add_facetracker.gif)

Objek **Face Tracker** akan automatis ditambahkan pada hierarki **Scene**
Jika diinginkan kamu juga dapat mengganti nama objek yang sudah kita buat dengan menekan key **F2** atau dengan klik kanan lalu pilih **Rename**

## Menambahkan Objek Plane
Setelah Face Tracker, sekarang kita membutuhkan sebuah objek yang akan menjadi tempat ditampilkannya gambar filter kita. Kita akan menambahkan sebuah objek dengan tipe Plane.

Untuk menambahkan **Plane** kita klik tombol **Add Object** pada panel **Scene**, lalu pilih **Plane** kemudian klik **Insert**

![add plane](tutorial_images/05_add_plane.gif)

Objek **Plane** telah ditambahkan pada panel **Scene** dan juga tampak pada panel **3D View**. Namun objek **Plane** masih diam tidak mengikuti gerakan wajah, ini akan kita perbaiki pada langkah selanjutnya.

![plane not move](tutorial_images/06_plane_not_move.gif)

## Mengatur Ulang Hierarki Objek
Untuk membuat objek **Plane** bisa bergerak sesuai dengan gerakan wajah, kita perlu mengatur ulang ususan hierarki objek pada **Scene**. Kita perlu memindahkan **Plane** masuk kedalam **Face Tracker** agar dapat bergerak bersama dengan gerakan wajah.

Untuk memindahkan, pada panel **Scene** drag dan drop objek **Plane** kedalam objek **Face Tracker**

![drag and drop](tutorial_images/07_plane_heriarchy.gif)

Dan hasilnya, objek **Plane** ikut bergerak sesuai gerakan wajah

![plane moving](tutorial_images/08_plane_moving.gif)

## Mengatur Posisi Objek
Jika kita perhatikan saat ini posisi objek **Plane** menutupi wajah, kita perlu mengatur posisi ini agar sesuai dengan yang kita inginkan. Ada beberapa cara yang bisa dilakukan yaitu dengan langsung menggeser objek melalui panel **3D View** atau dengan menggunakan input pada panel **Properties**

### 3D View
Memindah objek via **3D View** dapat dilakukan dengan menggeser menggunakan garis panah yang ada. Pertama untuk mempermudah menggeser objek, kita **Pause** kamera preview dengan menekan tombol pause disisi kiri layar

![pause](tutorial_images/09_pause_cam.gif)

Dan untuk menggeser tinggal klik objek pada panel **Scene** dan pada **3D View** arahkan garis panah objek ke posisi yang diinginkan.

![move arrow](tutorial_images/10_move_plane_arrow.gif)

### Properties
input2
