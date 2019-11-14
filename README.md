# latihan1
instal git
-download git, buka website resminya git (git-scm.com)
-kemudian unduh git sesuai dengan artistektur komputer kita, kalau menggunakan 64 bit,unduh yang 64 bit begitu jga kalau menggunakan 32 bit menggunakkan 32 bit.
-selamat,git sudah terinstal di windows, untuk mencobanya, silahkan buka cmd atau power shell, kemudian ketik perintah git --version.

menambahkan global config
-pada saat pertama kali menggunakan git,p perlu dilakukan konfigurasi user.name dan user email
-konfigurasi ini bisa dilakukan untuk global repository  atau individual repository 
-apabila belum dilakukan konfigurasi,akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit
-config global repository
$ git config --global user.name "name_user"
$ git config --global user.email "name_user"

membuat repository local
-buka directorry aktif, misal:d\labs_pemrograman1 (buka menggunakan windows explorer)
-klik kanan pada directorry aktif tersebut , dan pilih menu Git Bash, sehingga muncul git bash command
-buat directorry project pratikum pertama dengan nama latihan1 
$ mkdir latihan1
$ cd latihan1
-sehingga terbentuk satu directorry baru dibawahnya, selanjutnya masuk kedalam directorry tersebut dengan perintah cd(change directorry)
-directory aktif menjadi :d\labs_pemrograman1\latihan1

membuat repository local 
-jalankan perintah git init, untuk membuat reopsitory local.
$ git init
-repositorry baru berhasil di instalisasi, dengan terbentuknya satu directorry hidden dengan nam.git
-pada directorry tersebut, semua perubahan paada working directorry akan di simpan99

menambah file baru repository
-untuk membuat file dapat menngunakan text editor, lalu nilai menyimpan filenya pada directorry aktif(repository)
$echo "#latihan 1">>README.md
file README,md berhasil dibuat.

menambahkan file baru pada repository 
-untuk menambahkan file yang baru saja di buat tersebut gunakan perintah git add
$ add README.md

commit(menyimpan perubahan ke database)
-untuk menyimpan yang ada di dalam database respositorry local, gunakan perintah git commit m"komentar commit"
$ git commit m" file pertama saya"
-perubahan berhasil di simpan

membuat repositorry
-server repositorry yang akan kita gunakan adalah http://github.com
-anda harus membuat akun terlebih dahulu
-pada laman github, klik tombol start a project, atan
-dari menu (icon+)klik tombol repositorry 

membuat repositorry server
-isi nama repositorrynya, misal: labbpy1.
-lalu klik tombol creat repostitorry 

membuat remote repostitorry 
-remote repostitorry merupakan repostitorry server yabg akan di gunkkan untuk menyimpan setiap perubahan pada local repostitorry,sehingga dapat di akses oleh banyak user
-untuk memindahkan remote repostitorry server, gunakan perintah git remote add origun (url)
$ git remote add origin http://github.com/restu12345/latihan1.git

push (mengirim perubahan ke server)
-untuk mengirim pada local repostitorry ke server gunakan perintah git push
$ git push -u origin master
-perintah ini akan meminta memasukan user.name dan password pada akun github.com

melihat hasilnya pada server repostitorry
-buka lama githuub.com arahkan pada repostitorrynya
-maka perubuhan akan terlihat pada hallaman tersebut   
