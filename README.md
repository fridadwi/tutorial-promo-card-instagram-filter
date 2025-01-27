
# Overview

Dalam [laporan](https://www.ilo.org/wcmsp5/groups/public/---dgreports/---dcomm/documents/briefingnote/wcms_755910.pdf) ILO (International Labour Organisation) diprediksi terjadi pengurangan jam kerja setara dengan 495 juta full time job akibat dari pandemi Covid-19. Banyak orang yang akhirnya kehilangan pekerjaan.


![pandemi](tutorial_images/00_sad.gif)

Termasuk disini di Indonesia banyak orang kehilangan sumber pendapatannya akibat pandemi ini. Namun tidak sedikit yang mencoba mencari kesempatan baru dengan membuka usaha kecil. Berbagai cara dilakukan untuk mempromosikan usaha mereka dan tentunya sosial media menjadi platform favorit yang digunakan. Instagram sebagai salah satu sosial media dengan pengguna terbesar di Indonesia menjadi pilihan utama.

Salah satu fitur Instagram yang sangat diminati untuk promosi adalah **Instagram Story** dengan berbagai **Filter** menariknya. Dalam tutorial ini kita akan coba membuat sebuah **Filter** yang dapat digunakan untuk membantu promosi. **Filter** ini nantinya akan berbentuk **Promo Card** yang bisa dengan mudah dimodifikasi dengan gambar atau foto yang user siapkan sendiri untuk tiap program promosinya.

![filter](tutorial_images/00_sample.png)

Tutorial ini kami coba rancang untuk bisa diaplikasikan oleh user yang awam coding atau bahkan belum pernah menggunakan **Spark AR Studio**, sehingga semoga dapat membantu mereka yang sedang mencari kesempatan baru ditengah pandemi ini.

Beberapa hal yang akan dicakup dalam tutorial ini adalah :

* Persiapan dan cara menginstall **Spark AR Studio**
* Membuat **Filter** sederhana berupa **Promo Card** dengan fitur **Gallery Texture**, dimana nantinya user dapat menggunakan gambar atau fotonya sendiri pada **Filter**.
* Testing dan langkah-langkah untuk menerbitkan **Filter** yang telah kita buat.

Diharapkan setelah mengikuti tutorial ini kamu sudah bisa membuat filter mu sendiri yang dapat berfungsi dengan baik dan berhasil merilisnya.

# Daftar Isi
- [Overview](#overview)
- [Daftar Isi](#daftar-isi)
- [Menginstall Spark AR Studio](#-menginstall-spark-ar-studio)
  * [Persyaratan](#persyaratan)
    + [Hardware](#hardware)
    + [Akun](#akun)
    + [Download Installer](#download-installer)
    + [Login Facebook](#login-facebook)
- [Membuat Project Baru](#-membuat-project-baru)
  * [Membuka Blank Project](#membuka-blank-project)
  * [Tampilan utama Spark AR Studio](#tampilan-utama-spark-ar-studio)
  * [Menambahkan Face Tracker](#menambahkan-face-tracker)
  * [Menambahkan Objek Plane](#menambahkan-objek-plane)
  * [Mengatur Ulang Susunan Objek](#mengatur-ulang-susunan-objek)
  * [Mengatur Posisi Objek](#mengatur-posisi-objek)
    + [Menggunakan Panel View](#menggunakan-panel-view)
    + [Menggunakan Panel Properties](#menggunakan-panel-properties)
  * [Menambahkan Material](#menambahkan-material)
  * [Memasang Material Pada Objek](#memasang-material-pada-objek)
  * [Menambahkan fitur Gallery Texture](#menambahkan-fitur-gallery-texture)
  * [Memasang Texture Ke Material](#memasang-texture-ke-material)
  * [Memasang Holding Texture](#memasang-holding-texture)
  * [Mencoba Fitur Add Media](#mencoba-fitur-add-media)
- [Testing Filter Dan Menerbitkan Filter](#-testing-filter-dan-menerbitkan-filter)
  * [Testing Filter Pada Device](#testing-filter-pada-device)
    + [Testing menggunakan Spark AR Player](#testing-menggunakan-spark-ar-player)
    + [Testing menggunakan akun Instagram](#testing-menggunakan-akun-instagram)
  * [Menerbitkan Filter](#menerbitkan-filter)
    + [Upload dan Export](#upload-dan-export)
  * [Approval](#approval)
- [Apa selanjutnya?](#apa-selanjutnya)
- [Kesimpulan](#kesimpulan)
- [Kredit](#kredit)


# ![list](tutorial_images/00_list.gif) Menginstall Spark AR Studio

**Spark AR Studio** adalah platform augmented reality untuk Mac & Windows yang memungkinkan kita membuat efek AR untuk kamera seluler dengan mudah. Pada bagian ini kita akan mempersiapkan hal-hal yang dibutuhkan untuk penggunaan **Spark AR Studio** 

![prepare](tutorial_images/00_yuk.gif) 

## Persyaratan
Untuk menginstall **Spark AR Studio** ada beberapa hal yang perlu kita persiapkan.

### Hardware
**Spark AR Studio** membutuhkan PC dengan spesifikasi minimum seperti berikut
* Sistem Operasi minimum Windows 10 (64 bit) atau MacOS 10.14+
* RAM minimum 4GB

Spesifikasi lebih detail dapat dilihat pada laman https://sparkar.facebook.com/ar-studio/learn/downloads/#system-requirements

### Akun
Untuk menggunakan **Spark AR Studio** dan mempublikasikan **Filter** yang akan kita buat, dibutuhkan beberapa akun yaitu :
* Akun Facebook, untuk login dan menggunakan **Spark AR Studio** serta mengorganisir project yang akan kita terbitkan.
* Akun Instagram yang terkoneksi dengan akun Facebook tadi, untuk testing dan menerbitkan **Filter** yang kita buat.

### Download Installer
Apabila seluruh persyaratan telah terpenuhi sekarang kita bisa mulai install **Spark AR Studio** dengan mengunduh versi terbarunya di

https://sparkar.facebook.com/ar-studio/learn/downloads/#spark-ar-studio

Saat tutorial ini dibuat, versi terbaru yang digunakan adalah v98. Setelah berhasil mengunduh installer, silahkan install sesuai dengan langkah-langkah yang ditampilkan.

### Login Facebook
Hal yang akan muncul saat kita pertama kali membuka **Spark AR Studio** adalah popup login akun Facebook, isilah dengan data akunmu dan kemudian kamu dapat menggunakan **Spark AR Studio**.

![login](tutorial_images/00_login.PNG)

Untuk logout **Spark AR Studio** dari akun yang digunakan saat ini, bisa dilakukan setelah membuka project dengan cara : klik **File** lalu pilih **Logout**.

Ini adalah akhir bagian pertama dari total 3 bagian tutorial. Kamu sudah berhasil menyiapkan **Spark AR Studio** untuk membuat **Filter** yang akan dibahas pada bagian kedua tutorial ini. 

![goodjob](tutorial_images/00_mantap.png) 

# ![list](tutorial_images/00_list.gif) Membuat Project Baru

Pada bagian ini kita akan mulai untuk membuat project Filter.

![start project](tutorial_images/00_start.gif) 

Silahkan buka **Spark AR Studio** yang sudah di install, tampilan awal dari **Spark AR Studio** adalah list beberapa template yang disediakan, dan terdapat beberapa tutorial yang nanti bisa kamu coba-coba sendiri.

![homepage](tutorial_images/01_homepage.PNG)

## Membuka Blank Project

Untuk saat ini kita akan memulai dengan membuat project baru dari awal.

Klik **Create New** > **New Project**.

Akan ditampilkan popup tipe project yang bisa kamu buat. Karena saat ini kita akan belajar dari awal, maka pilihlah **Blank Project**.

![project baru](tutorial_images/02_new_project.gif)


## Tampilan utama Spark AR Studio
**Spark AR Studio** akan membuka sebuah window baru yang akan menjadi workarea kita. Jika diperhatikan, workarea kita terbagi menjadi beberapa area utama.

![mainview](tutorial_images/03_Main_View.PNG)

- A adalah panel **Scene**. Panel **Scene** berguna untuk mengatur urutan objek-objek yang akan kita gunakan. Secara default sudah disiapkan Ambient Light dan Directional Light. Untuk project ini akan kita abaikan saja kedua objek light tersebut.
- B adalah panel **Assets**. Panel **Assets** akan kita gunakan untuk mengorganisir file yang kita gunakan pada project, seperti Image dan Material.
- C adalah panel **View**. Pada bagian tengah akan menjadi workarea utama dimana kita bisa melihat dan mengedit secara langsung posisi dan ukuran objek-objek pada project kita. Disediakan juga sebuah window **Simulator** sebagai contoh bagaimana tampilan di device.
- D adalah panel **Properties**. Pada sisi kanan tersedia panel **Properties** yang bisa digunakan untuk mengatur setting dari object yang kita gunakan.

## Menambahkan Face Tracker
Mendeteksi wajah adalah hal utama yang kita butuhkan untuk membuat **Filter** ini, dengan menggunakan **Spark AR Studio** fitur ini sangat mudah kita buat karena **Spark AR Studio** telah menyediakan beberapa jenis tracker diantaranya **Face Tracker**.

Untuk menggunakan Face Tracker sangatlah mudah, pada panel **Scene** klik tombol **Add Object** yang berada di sisi kanan bawah lalu pilih **Face Tracker** kemudian klik **Insert**.

![add face tracker](tutorial_images/04_add_facetracker.gif)

Objek **Face Tracker** akan automatis ditambahkan pada daftar objek pada panel **Scene**.
Jika diinginkan kamu juga dapat mengganti nama objek yang sudah kita buat dengan klik dua kali atau dengan klik kanan lalu pilih **Rename**.

## Menambahkan Objek Plane
Setelah Face Tracker, sekarang kita membutuhkan sebuah objek yang akan menjadi tempat ditampilkannya gambar filter kita. Kita akan menambahkan sebuah objek dengan tipe Plane.

Untuk menambahkan **Plane** kita klik tombol **Add Object** pada panel **Scene**, lalu pilih **Plane** kemudian klik **Insert**.

![add plane](tutorial_images/05_add_plane.gif)

Objek **Plane** telah ditambahkan pada panel **Scene** dan juga tampak pada panel **View**. Namun objek **Plane** masih diam tidak mengikuti gerakan wajah, ini akan kita perbaiki pada langkah selanjutnya.

![plane not move](tutorial_images/06_plane_not_move.gif)

## Mengatur Ulang Susunan Objek
Untuk membuat objek **Plane** bisa bergerak sesuai dengan gerakan wajah, kita perlu mengatur ulang susunan objek pada **Scene**. Kita perlu memindahkan **Plane** masuk kedalam **Face Tracker** agar dapat bergerak bersama dengan gerakan wajah.

Untuk memindahkan, pada panel **Scene** drag dan drop objek **Plane** kedalam objek **Face Tracker**.

![drag and drop](tutorial_images/07_plane_heriarchy.gif)

Dan hasilnya, objek **Plane** ikut bergerak sesuai gerakan wajah.

![plane moving](tutorial_images/08_plane_moving.gif)

## Mengatur Posisi Objek
Jika kita perhatikan saat ini posisi objek **Plane** menutupi wajah, kita perlu mengatur posisi ini agar sesuai dengan yang kita inginkan. Ada beberapa cara yang bisa dilakukan yaitu dengan langsung menggeser objek melalui panel **View** atau dengan menggunakan input pada panel **Properties** yang terdapat disisi kanan layar.

### Menggunakan Panel View
Memindah objek via **View** dapat dilakukan dengan menggeser menggunakan garis panah yang ada. Pertama untuk mempermudah menggeser objek, kita **Pause** kamera **Simulator** dengan menekan tombol pause disisi kiri layar.

![pause](tutorial_images/09_pause_cam.gif)

Dan untuk menggeser tinggal klik objek pada panel **Scene** dan pada **View** arahkan garis panah objek ke posisi yang diinginkan.

![move arrow](tutorial_images/10_move_plane_arrow.gif)

### Menggunakan Panel Properties
Untuk memindahkan objek dengan lebih persisi kita bisa menggunakan panel **Properties**. Sebagai contoh kita klik objek pada panel **Scene** dan pada panel **Properties** yang terdapat disisi kanan layar kita ubah nilai Position Y menjadi 0.1 sehingga posisi objek **Plane** berpindah ke dahi.

![move properties](tutorial_images/11_move_plane_properties.gif)


Selain untuk memindahkan objek, cara-cara tadi juga bisa digunakan untuk mengubah ukuran dan rotasi objek. Silahkan dicoba-coba.
Selanjutnya kita akan menambahkan **Material** agar objek dapat memiliki warna atau gambar.

## Menambahkan Material

Jika kita perhatikan objek **Plane** saat ini ditampilkan dalam warna kotak catur hitam-putih, itu artinya objek **Plane** belum memiliki data yang akan ditampilkan pada layar. Untuk memberikan tampilan pada objek **Plane** kita membutuhkan sebuah aset yang disebut **Material**.

**Material** adalah aset yang akan mengontrol bagaimana sebuah objek akan ditampilkan pada layar. **Material** bisa menampilkan warna, gambar, atau juga animasi.

Untuk menambahkan **Material** klik tombol **Add Asset** pada panel **Assets** lalu pilih **Material**.

![add material](tutorial_images/12_add_material.gif)

## Memasang Material Pada Objek

Setelah memiliki aset **Material** langkah selanjutnya akan kita pasangkan **Material** tersebut ke objek **Plane**.

Seleksi objek **Plane** pada panel **Scene**, lalu pada panel **Properties** yang terdapat disisi kanan layar perhatikan bagian **Materials**. Klik tombol **+** untuk memilih **Material** yang sudah kita siapkan.

![place material](tutorial_images/13_place_material.gif)

Setelah dipasangkan **Material**, objek **Plane** berubah warna menjadi putih, mengikuti pengaturan **Material** yang diberikan.

![white plane](tutorial_images/13a_white_material.gif)

Pada bagian selanjutnya kita akan menambahkan fungsi mengambil gambar dari file milik user dan memasangnya kedalam **Material** yang sudah dibuat, sehingga nanti user bisa membuat gambar Promo Card-nya sendiri.

## Menambahkan fitur Gallery Texture

**Gallery Texture** adalah fitur dari **Spark AR Studio** yang memungkinkan kita untuk menggunakan file dari Gallery user sebagai material. Untuk saat tutorial ini dibuat, fitur ini hanya bisa digunakan untuk platform Instagram.

Untuk menambahkan **Gallery Texture**, pada panel **Assets** klik **Add Asset** dan pilih **Gallery Texture**.

![add gallery texture](tutorial_images/14_add_gallery_texture.gif)

Biasanya akan muncul sebuah **Warning Popup**, artinya kita perlu mengnonaktifkan Facebook pada Platform yang kita tuju. Klik tombol **Review Platform** lalu hilangkan tanda centang pada opsi Facebook, kemudian klik **Done** untuk menyelesaikan.

![add gallery texture](tutorial_images/15_capability_popup.gif)

Selanjutnya kita ulangi kembali proses menambahkan **Gallery Texture**.

![add gallery texture](tutorial_images/14_add_gallery_texture.gif)

Setelah **Gallery Texture** ditambahkan, pada **Simulator** akan muncul tombol **Add Media** yang nantinya bisa digunakan oleh user untuk memilih gambar yang dimiliki.

![add media button](tutorial_images/17_add_media_button.PNG)

## Memasang Texture Ke Material

Saat ini yang terlihat pada objek **Plane** adalah warna putih dari **Material** yang kita punya. Untuk langkah selanjutnya adalah kita akan mencoba memasang texture dari **Gallery Texture** ke **Material** tersebut agar gambar yang nantinya dipilih oleh user dapat ditampilkan pada objek **Plane**.

Klik **Material** yang akan diubah pada panel **Assets**. Pada panel **Properties** yang terdapat disisi kanan layar perhatikan bagian **Shader Properties**, pada **Texture** klik drop down button dan pilih **galleryTexture0** yang merupakan nama asset **Gallery Texture** kita.

![texture to material](tutorial_images/18_add_texture_to_material.gif)

Jika kita perhatikan, objek **Plane** yang semula berwarna putih berubah menjadi berwarna kotak catur kembali. Hal ini dikarenakan **Gallery Texture** belum memiliki data yang akan ditampilkan.

Pada langkah selanjutnya kita akan memasang sebuah gambar default yang akan ditampilkan sebelum user memilih gambarnya sendiri.

## Memasang Holding Texture

Klik **Gallery Texture** pada panel **Assets**, pada panel **Properties** yang terdapat disisi kanan layar berikan centang pada **Holding Texture** dan klik **Choose File**.

Pilihlah file gambar yang akan kamu gunakan. Kamu juga bisa menggunakan gambar yang bisa diunduh pada [link ini](Assets.zip).

![holding texture](tutorial_images/19_add_holding_image.gif)

Seperti nampak pada **Simulator**, objek **Plane** saat ini sudah memiliki texture default berupa image yang kita pilih tadi.

## Mencoba Fitur Add Media

Kita bisa coba klik tombol **Add Media** untuk mencoba mengubah default image dengan file yang kita punya.

![test the button](tutorial_images/20_test_add_media.gif)

tombol inilah yang nantinya memungkinkan user menggunakan file mereka sendiri pada **Filter** yang kita buat.

Selamat! **Filter** yang kita buat sudah hampir jadi, langkah selanjutnya adalah mencobanya pada device secara langsung untuk memastikan tidak ada kendala dalam penggunaannya. Hal ini akan kita lakukan pada bagian selanjutnya.

![goodjob](tutorial_images/00_mantap.png) 



# ![list](tutorial_images/00_list.gif) Testing Filter Dan Menerbitkan Filter

Testing sebelum menerbitkan **Filter** adalah salah satu langkah paling penting untuk memastikan **Filter** yang kita buat berjalan dengan baik dan sesuai dengan apa yang kita rencanakan.

## Testing Filter Pada Device

Ada dua cara untuk melakukan testing pada device :
- Dengan menginstall Spark AR Player pada device
- Dengan menggunakan akun Instagram pada device

### Testing menggunakan Spark AR Player

Aplikasi **Spark AR Player** tersedia untuk Android dan IOS, bisa kamu download terlebih dahulu melalui link yang tersedia di https://sparkar.facebook.com/ar-studio/learn/downloads/#spark-ar-player-app.

Setelah terinstall, hubungkan device dengan PC menggunakan USB.

Pada **Spark AR Studio** bagian kiri bawah terdapat beberapa button, klik pada button **Test On Device**.

Tunggu hingga muncul nama device, jika sudah muncul klik tombol **Send**. **Filter** automatis dijalankan pada device.

![apps preview](tutorial_images/21_preview_apps.gif)

Apabila nama device tidak muncul, coba ulangi hubungkan device dengan PC menggunakan USB.

### Testing menggunakan akun Instagram
Pada **Spark AR Studio** bagian kiri bawah terdapat beberapa button, klik pada button **Test On Device**. Pada bagian **Send to App** klik **Send** pada **Instagram Camera**.

![instagram preview](tutorial_images/22_preview_instagram.gif)

Apabila telah terkirim periksa Instagram pada devicemu, akan muncul notifikasi yang bisa kamu tap untuk mencoba **Filter** yang sudah kamu buat.

![notification](tutorial_images/23_notification.png)

Sebenarnya kita juga bisa testing menggunakan akun Facebook (Facebook Camera), tetapi karena kita menggunakan fitur **Gallery Texture** yang hanya bisa diaplikasikan pada Instagram maka opsi Facebook Camera tidak ditampilkan.

## Menerbitkan Filter

Sebelum memulai proses penerbitan, kita perlu mempersiapkan Icon dan Video demo. 
* Beberapa syarat icon yang diperlukan adalah :
   * File dalam format PNG atau JPG.
   * Tidak menggunakan *rounded corner*.
   * *Color space* yang digunakan sRGB.
   * Minimal berukuran 200 x 200 pixel.
   * Tanpa menggunakan transparansi.
   * Tidak menggunakan warna gradasi Instagram.
   
   Untuk membuat icon yang sesuai dengan persyaratan silahkan cek penjelasannya di https://sparkar.facebook.com/ar-studio/learn/publishing/icons-and-names-for-spark-ar-effects. Disana juga tersedia template icon yang bisa kamu pakai agar sesuai dengan syarat yang berlaku.
    
* Beberapa syarat video demo yang diperlukan adalah:
   * Direkam dan disimpan langsung dari kamera Instagram.
   * Tidak diedit (jangan gunakan video Boomerang, jangan beri teks tambahan).
   * Rekam dalam bentuk vertikal.
   * Durasi maksimal 15 detik.
   * Besar file maksimal 34MB.
   * Upload dalam bentuk file MP4 atau MOV.
   
   Untuk membuat video demo yang sesuai dengan persyaratan silahkan cek penjelasannya di https://sparkar.facebook.com/ar-studio/learn/publishing/demo-videos-for-instagram-effects.

### Upload dan Export

Setelah menyiapkan icon dan video demo, langkah selanjutnya adalah upload project ke **Spark AR Hub** untuk bisa diterbitkan.

Pada **Spark AR Studio** pada bagian kiri bawah terdapat beberapa button, klik pada button **Upload and Export**. Kemudian klik **Upload** pada popup window yang muncul. Tunggu proses uploading hingga selesai.

![export and upload](tutorial_images/23_export_and_upload.gif)

Setelah proses upload selesai kita akan diarahkan ke laman **Spark AR Hub**.

![spark ar hub](tutorial_images/24_spark_ar_hub.png)

Inputlah informasi dan file-file yang dibutuhkan. Beberapa hal yang perlu diperhatikan antara lain :
* Pada **Platform** hanya aktifkan **Instagram**, karena fitur **Gallery Texture** tidak tersedia di Facebook.
* Pada **Categories** pilihlah kategori yang relevan dengan **Filter** yang kita buat, untuk project ini bisa dipilih **Appearence and Selfies**.
* Pada **Publication date** bisa dipilih apakah akan segera dirilis ketika mendapat persetujuan atau ingin dijadwalkan di waktu yang lain.

![spark ar hub completed](tutorial_images/25_spark_ar_hub_complete.png)

Setelah seluruh form terisi, untuk melanjutkan klik tombol **Submit** yang berada di sisi kanan atas laman **Spark AR Hub**. Apabila belum berhasil menyelesaikan pengisian form bisa klik tombol **Save** dan dilanjutkan pada kesempatan lain dengan mengakses laman https://www.facebook.com/sparkarhub/effects/.

Setelah selesai melakukan submisi, kita tinggal menunggu **Filter** yang kita buat mendapat approval.

## Approval

Sebelum **Filter** bisa digunakan oleh masyarakat luas, **Filter** akan melalui proses **Review** dengan jangka waktu antara 1 hingga beberapa hari.

Apabila **Filter** kita mendapatkan penolakan akan muncul notifikasi di **Facebook** dan **Spark AR Hub**, silahkan diperiksa alasan penolakannya dan lakukan perbaikan yang dibutuhkan. Setelah seluruh perbaikan dilakukan kita bisa melakukan submisi kembali.

Apabila **Filter** kita mendapat persetujuan juga akan muncul notifikasi di **Facebook** dan **Spark AR Hub**.

![notification](tutorial_images/28_approval_notif.png)

Untuk menggunakan **Filter** yang sudah mendapat persetujuan, kita bisa dapatkan link **Filter** pada **Spark AR Hub**.

![spark ar hub link](tutorial_images/26_filter_link.png)

Atau bisa diakses melalui **Tab Filter** pada akun **Instagram** kita, tab yang ditandai dengan icon wajah.

![instagram filter tab](tutorial_images/27_filter_on_instagram.png)

Dengan mendapat approval artinya **Filter** yang kita buat sudah bisa digunakan oleh publik untuk membuat **Instagram Story**.

Selamat! kamu sudah menyelesaikan seluruh langkah-langkah untuk membuat **Filter** menggunakan **Spark AR Studio**.
 
![goodjob](tutorial_images/00_berhasil.png) 

# Apa selanjutnya?
Jika kamu tertarik mengembangkan Instagram Filter lebih dalam, kamu bisa mengunjungi tautan berikut untuk mencoba tutorial menarik atau mendapatkan informasi lainnya.

- https://sparkar.facebook.com/ar-studio/learn/
- https://www.facebook.com/SparkARcreators/

Kamu juga bisa bergabung dengan **[Spark AR Community](https://www.facebook.com/groups/SparkARcommunity "Spark AR Community")** untuk berdiskusi dan berbagi informasi pengembangan Filter dengan Spark AR Studio


# Kesimpulan

Membuat Instagram Filter dapat dengan mudah dilakukan oleh siapapun dengan bantuan **Spark AR Studio** dengan semua fitur-fiturnya. Banyak hal yang bisa dikembangkan dan semoga bisa menjadi peluang baru di masa pandemi ini.


# Kredit
Pembuat :
- Frida Dwi (Tutorial) https://www.instagram.com/ultrmnbstrd/
- Estu Galih (2D Artist) https://www.instagram.com/nekozilla/

Tutorial ini terinspirasi dari :
- https://sparkar.facebook.com/ar-studio/learn/articles/textures-and-materials/gallery-texture-and-gallery-picker
