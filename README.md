# Latihan--VCS

NAMA : DANI DARSONO

NIM : 312010189

KELAS : TI.20.B1

DOSEN : Agung Nugroho,S.Kom.,M.Kom

Tugas : Membuat satu repository LatihanVCS dan Buat file README.md

Instalasi Git

• Download Git, buka website resminya Git (git-scm.com).
 
![1](https://user-images.githubusercontent.com/73014427/96397269-625e3b80-11f3-11eb-83b9-890209c0f048.png)


• Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit.

![2](https://user-images.githubusercontent.com/73014427/96397756-6179d980-11f4-11eb-9f12-5866977ba06f.png)




![3](https://user-images.githubusercontent.com/73014427/96400866-195eb500-11fc-11eb-889f-c8aaf88706b6.png)



• Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah



git --version

![4](https://user-images.githubusercontent.com/73014427/96402468-28476680-1200-11eb-9b66-5e84d08bab9e.png)



Menambahkan Global Config

• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

• konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

• Config Global Repository

$ git config --global user. name “nama_user”

$ git config --global user. email “nama_user”


![5](https://user-images.githubusercontent.com/73014427/96402520-575dd800-1200-11eb-8cec-e00b486dad99.png)

Membuat Reposiory Local

• Buka direktory aktif, misal: e:\labs_pemrograman1 (buka menggunakan Windows Explorer)

• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

• Buat direktory project praktikum pertama dengan nama Latihan-VCS

$ mkdir Latihan-VCS

$ cd Latihan-VCS

 
![6](https://user-images.githubusercontent.com/73014427/96402620-92600b80-1200-11eb-9996-5182bb53277c.png)



• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)

• direktory aktif menjadi: e:\labs_pemrograman1\Latihan-VCS

Membuat Reposiory Local

• Jalankan perintah git init, untuk membuat repository local.

$ git init

![7](https://user-images.githubusercontent.com/73014427/96402805-026e9180-1201-11eb-9a9e-074f67bcb9f1.png)



• Repository baru berhasil di inisialisasi, dengan terbentuknya satu Direktori hidden dengan nama .git 

![8](https://user-images.githubusercontent.com/73014427/96402895-31850300-1201-11eb-9a4e-e7e147854b4c.png)


• Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

Menambahkan File baru pada repository

• Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

• disini kita akan coba buat satu file bernama README.md (text file)

$ echo “# Latihan-VCS” >> README. md

![9](https://user-images.githubusercontent.com/73014427/96403191-e15a7080-1201-11eb-97fa-d1e92998c952.png)

• File README.md berhasil dibuat.

![10](https://user-images.githubusercontent.com/73014427/96403270-18c91d00-1202-11eb-9dbb-2e8c6b471499.png)



Menambahkan File baru pada repository

• Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

$ git add README. md

• File README.md berhasil ditambahkan

![11](https://user-images.githubusercontent.com/73014427/96403324-4b731580-1202-11eb-9849-f8aa0d79ed62.png)


Commit (Menyimpan perubahan ke database)

• Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”

$ git commit -m “Bahasa Pemrograman Repository Lokal LatihanVCS"

![12](https://user-images.githubusercontent.com/73014427/96403409-870ddf80-1202-11eb-8b0c-74e309711b76.png)


• Perubahan berhasil disimpan.

![13](https://user-images.githubusercontent.com/73014427/96403481-bd4b5f00-1202-11eb-9b1a-a9df3c990ecb.png)



Membuat repository server

• Server reopsitory yang akan kita gunakan adalah http://github.com

• Anda harus membuat akun terlebih dahulu.

• Pada laman github, klik tombol start a project, atau

• Dari menu (icon +) klik New Repository

![14](https://user-images.githubusercontent.com/73014427/96403574-f4ba0b80-1202-11eb-976d-68f9341dcaa6.png)


Membuat repository server

• Isi nama repositorynya, misal: LatihanVCS.


![15](https://user-images.githubusercontent.com/73014427/96403670-2337e680-1203-11eb-9662-c49b7c0b364f.png)


• lalu klik tombol Create repository


![16](https://user-images.githubusercontent.com/73014427/96404701-c689fb00-1205-11eb-8215-45dff73dc0c0.png)

Menambahkan Remote Repository

• Remote Repository merupakan repository server yang akan

digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

Alamat url kita

![17](https://user-images.githubusercontent.com/73014427/96404808-05b84c00-1206-11eb-9571-564b9c06487c.png)


• Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

$ git remote add origin https://github.com/danidarsono33/Latihan-VCS.git


![18](https://user-images.githubusercontent.com/73014427/96404885-34cebd80-1206-11eb-8f6a-31c223c613c1.png)

Push (Mengirim perubahan ke server)

• Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

$ git push -u origin master

• Perintah ini akan meminta memasukkan username dan password pada akun github.com

!GAMABAR 19

pada repositorinya.
Melihat hasilnya pada server repository

• Buka laman github.com, arahkan
• Maka perubahan akan terlihat pada laman tersebut.

!GAMBAR 20

!GAMBAR 21

Clone Repository

• Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).

• Untuk melakukan cloning, gunakan perintah git clone [url]

$ git clone https://github.com/danidarsono33/Latihan-VCS.git

!GAMBAR 22



Kegunaan file README.md

• Apabila kita menggunakan github, untuk memberikan penjelasan awal pada project yang kita buat, maka dapat menggunakan sebuah file yang bernama README.md

• Pada file tersebut kita dapat membuat dokumentasi awal dari setiap project yang kita buat untuk memberikan penjelasan atau sekedar cara penggunaan dari aplikasi yang kita kembangkan.

• Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan Markdown format.

• untuk lebih jelasnya, dapat anda gunakan cara penggunaan markdown

TERIMA KASIH😊

















