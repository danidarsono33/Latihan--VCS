# Latihan--VCS

NAMA : DANI DARSONO

NIM : 312010189

KELAS : TI.20.B1

DOSEN : Agung Nugroho,S.Kom.,M.Kom

Tugas : Membuat satu repository LatihanVCS dan Buat file README.md

Instalasi Git

• Download Git, buka website resminya Git (git-scm.com).
 
![1](https://user-images.githubusercontent.com/73014427/96397269-625e3b80-11f3-11eb-83b9-890209c0f048.png)


• Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit. 01_download git 02_istall git 03_git bash

![2](https://user-images.githubusercontent.com/73014427/96397756-6179d980-11f4-11eb-9f12-5866977ba06f.png)


• Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah

!GAMBAR 3

git --version
Menambahkan Global Config

• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

• konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

• Config Global Repository

$ git config --global user. name “nama_user”

$ git config --global user. email “nama_user”

!GAMBAR 4

Membuat Reposiory Local

• Buka direktory aktif, misal: e:\labs_pemrograman1 (buka menggunakan Windows Explorer)

• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

• Buat direktory project praktikum pertama dengan nama Latihan-VCS

$ mkdir Latihan-VCS

$ cd Latihan-VCS
 
!GAMBAR 5

• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)

• direktory aktif menjadi: e:\labs_pemrograman1\Latihan-VCS

Membuat Reposiory Local

• Jalankan perintah git init, untuk membuat repository local.

$ git init

!GAMBAR 6


• Repository baru berhasil di inisialisasi, dengan terbentuknya satu Direktori hidden dengan nama .git 

!GAMBAR 7

• Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

Menambahkan File baru pada repository

• Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

• disini kita akan coba buat satu file bernama README.md (text file)

$ echo “# Latihan-VCS” >> README. md

!GAMBAR 8

• File README.md berhasil dibuat.

!GAMBAR 9


Menambahkan File baru pada repository

• Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

$ git add README. md

• File README.md berhasil ditambahkan

!GAMBAR 10

Commit (Menyimpan perubahan ke database)

• Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”

$ git commit -m “Bahasa Pemrograman Repository Lokal LatihanVCS"

!GAMBAR 11

• Perubahan berhasil disimpan.

!GAMBAR 12

Membuat repository server

• Server reopsitory yang akan kita gunakan adalah http://github.com

• Anda harus membuat akun terlebih dahulu.

• Pada laman github, klik tombol start a project, atau

• Dari menu (icon +) klik New Repository

!GAMBAR 13

Membuat repository server

• Isi nama repositorynya, misal: LatihanVCS.


!GAMBAR 14

• lalu klik tombol Create repository


!GAMBAR 15

Menambahkan Remote Repository

• Remote Repository merupakan repository server yang akan

digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

Alamat url kita

!GAMBAR 16

• Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

$ git remote add origin https://github.com/danidarsono33/Latihan-VCS.git


!GAMBAR 17

Push (Mengirim perubahan ke server)

• Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

$ git push -u origin master

• Perintah ini akan meminta memasukkan username dan password pada akun github.com

!GAMABAR 18

pada repositorinya.
Melihat hasilnya pada server repository

• Buka laman github.com, arahkan
• Maka perubahan akan terlihat pada laman tersebut.

!GAMBAR 19

!GAMBAR 20

Clone Repository

• Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).

• Untuk melakukan cloning, gunakan perintah git clone [url]

$ git clone https://github.com/danidarsono33/Latihan-VCS.git

!GAMBAR 21



Kegunaan file README.md

• Apabila kita menggunakan github, untuk memberikan penjelasan awal pada project yang kita buat, maka dapat menggunakan sebuah file yang bernama README.md

• Pada file tersebut kita dapat membuat dokumentasi awal dari setiap project yang kita buat untuk memberikan penjelasan atau sekedar cara penggunaan dari aplikasi yang kita kembangkan.

• Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan Markdown format.

• untuk lebih jelasnya, dapat anda gunakan cara penggunaan markdown

TERIMA KASIH😊

















