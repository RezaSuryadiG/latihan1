#latihan 1
" Latihan 1 "

Menambahkan Global Config
Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email • konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository. • apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

Config Global Repository $ git config --global user.name “nama_user” $ git config --global user.email “nama_user”

Membuat Reposiory Local

Buka direktory aktif, misal: c:\user\iip\lab_pemrograman (buka menggunakan Windows Explorer)

klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash command

Buat direktory project praktikum pertama dengan nama latihan1 $ mkdir latihan1 $ cd latihan1

Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory) • direktory aktif menjadi: c:\user\iip\lab_pemrograman\latihan1

Jalankan perintah git init, untuk membuat repository local. $ git init

Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git

Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

Menambahkan File baru pada repository

Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

disini kita akan coba buat satu file bernama README.md (text file) $ echo “#Latihan 1” >> README.md

File README.md berhasil dibuat.



![Capture1](https://user-images.githubusercontent.com/56528282/66887875-a9c15300-f006-11e9-88a9-84243d9f8426.PNG)




Menambahkan File baru pada repository

Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add. $ git add README.md

File README.md berhasil ditambahkan.



![Capture2](https://user-images.githubusercontent.com/56528282/66887984-150b2500-f007-11e9-9de0-ff3456a8047c.PNG)




Commit (Menyimpan perubahan ke database)

Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit” $ git commit -m “File pertama saya”


![Capture3](https://user-images.githubusercontent.com/56528282/66888024-3a982e80-f007-11e9-8c90-e2c48eb943eb.PNG)



perubahan berhasil disimpan
Membuat repository server

Server reopsitory yang akan kita gunakan adalah http://github.com • Anda harus membuat akun terlebih dahulu.

Pada laman github, klik tombol start a project, atau

Dari menu (icon +) klik New Repositori.


![Capture4](https://user-images.githubusercontent.com/56528282/66888063-60253800-f007-11e9-96f5-36ce9d2deea2.PNG)



Isi nama repositorynya, misal: lab_prog1.

lalu klik tombol Create repositor.


![Capture5](https://user-images.githubusercontent.com/56528282/66888080-6f0bea80-f007-11e9-8e2f-eae5139221c8.PNG)




Menambahkan Remote Repository

Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url] $ git remote add origin https://github.com/RezaSuryadiG/latihan1

Push (Mengirim perubahan ke server)

Untuk mengirim perubahan pada local repository ke server gunakan perintah git push. $ git push -u origin master

Perintah ini akan meminta memasukkan username dan password pada akun github.com


![Capture6](https://user-images.githubusercontent.com/56528282/66888183-c01bde80-f007-11e9-923b-cf5214b4a002.PNG)





Melihat hasilnya pada server repository

Buka laman github.com, arahkan pada repositorinya.

Maka perubahan akan terlihat pada laman tersebut.

![Capture7](https://user-images.githubusercontent.com/56528282/66888198-d164eb00-f007-11e9-8f11-c2516cf4da14.PNG)








Clone Repository

Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).

Untuk melakukan cloning, gunakan perintah git clone [url]
![Capture8](https://user-images.githubusercontent.com/56528282/66888220-e6417e80-f007-11e9-8c2f-6c419232b25f.PNG)
