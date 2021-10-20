# **Cara Menginstall dan Menggunakan Git**
Pada Windows penginstallan git dilakukan dengan urutan sebagai berikut:

Buka Website https://git-scm.com -> Klik download file -> Klik kanan file yg sudah terinstall -> Klik run as administrator -> next 3x -> Finish

Berbeda dengan MacOs yang harus menginstall Brew terlebih dahulu, caranya sebagai berikut:

Buka Terminal pada Launchpad -> Masukan Link dari website brew.sh dibrowser -> copy link yang tertera pada beranda web -> paste link di terminal MacOs
-> masukan password mac kalian -> pencet tombol return -> tunggu sampai proses instalasi selesai -> ketika sudah selesai ketik "brew install git" pada terminal -> finish

## **1. Login Git di Terminal**
Untuk login ke Git, kita bisa menggunakan akun GitHub. Jika belum memiliki akun kita bisa mendaftarkan diri terlebih dahulu. 
Selanjutnya kita bisa melakukan login awal pada Git  menggunakan Terminal desktop anda . Kemudian masukkan perintah-perintah yang akan saya jelaskan di bawah ini.
Masukkan username GitHub kalian menggunakan perintah di bawah ini:

$ git config --global user.name "UsernameAnda"

Lalu tekan ENTER

Kemudian masukkan email yang terdaftar di GitHub kalian menggunakan perintah di bawah  ini:

$ git config --global user.email emailkalian@gmail.com

Lalu tekan ENTER

Selanjutnya untuk memastikan proses login kalian berhasil, masukkan perintah berikut:

$ git config –-list

![Jepretan Layar 2021-10-21 pada 03 56 49](https://user-images.githubusercontent.com/92860030/138172525-a057cec9-b273-4483-913a-9530c7cee1d0.png)

### **2. Login di Github.com**

Langkah kedua dalam belajar menggunakan Git adalah kalian harus login ke dalam website GitHub. 
Github dan Git memiliki hubungan khusus, yaitu Git yang berperan sebagai version control system dan 
Github menjadi hosting atau sebagai penyimpan kode pemrograman. Setelah kalian klik login, 
akan muncul tampilan dashboard dari GitHub seperti  gambar di bawah ini.
![Jepretan Layar 2021-10-21 pada 01 14 33](https://user-images.githubusercontent.com/92860030/138174026-4a66df1f-15d0-4fe3-8c84-ade49be5dc80.png)
#### **3. Buat Repository**

Setelah berhasil login ke GitHub, Anda bisa mulai membuat repository. 
Klik tombol "Create Repository" pada menu Repositories untuk membuat repository baru.
![Jepretan Layar 2021-10-21 pada 01 15 02](https://user-images.githubusercontent.com/92860030/138173218-8cc136da-7745-4040-9f46-0ea2ff3f919d.png)

Kemudian Anda akan diarahkan pada halaman untuk membuat repository baru seperti gambar di bawah ini. 
![Jepretan Layar 2021-10-21 pada 01 32 20](https://user-images.githubusercontent.com/92860030/138174301-1a958121-23fd-4949-b3ce-8b19839a6051.png)
Anda perlu mengisi detail informasi berikut:

•	Nama Repository : digunakan untuk identitas repository yang dibuat.

•	Deskripsi Repository : berfungsi untuk deskripsi dari repository yang dibuat.

•	Jenis Repository   : jenis repository  dibagi menjadi Public dan Private. 

Ketika Anda mengatur repository menjadi Public, orang lain dapat melihat repository yang kalian buat.
Sebaliknya, jika kalian mengaturnya sebagai Private, repository tersebut hanya bisa diakses oleh kalian.
Setelah mengisi detail informasi di atas, klik Create Repository.

##### **4. Buat Folder pada Dekstop**
Selanjutnya, kalian perlu membuat folder pada local disk komputer kalian. 
Fungsinya adalah untuk menyimpan update file dari repository GitHub yang telah kalian buat.

Buka Finder -> Klik Dekstop -> Klik logo setting -> Klik Folder Baru -> Beri nama folder -> Selesai
![Jepretan Layar 2021-10-21 pada 01 37 30](https://user-images.githubusercontent.com/92860030/138174849-1006192b-50f6-4533-8d2f-ea28ad473f87.png)
###### **5. Buka Folder Menggunakan Git Bash**
Setelah berhasil membuat folder pada local disk komputer kalian, 
karena milik saya MacOs jadi folder pada local disk saya tarik dan tempel ke terminal/git bash langsung. 
Jika pada windows buka folder tersebut dengan cara klik kanan lalu pilih Git Bash Here.

![Jepretan Layar 2021-10-21 pada 04 30 11](https://user-images.githubusercontent.com/92860030/138175160-82086123-34cf-49b4-81b9-33381d728970.png)

Setelah itu, Command Prompt akan muncul seperti di bawah ini. 

![Jepretan Layar 2021-10-21 pada 01 54 06](https://user-images.githubusercontent.com/92860030/138175344-371751e5-a100-483b-b58c-b798558158fa.png)

**6. Ubah Folder Menjadi Repository**

Setelah itu, ubah folder tersebut menjadi repository menggunakan perintah berikut:

$ git init

![Jepretan Layar 2021-10-21 pada 01 56 47](https://user-images.githubusercontent.com/92860030/138175599-7f736945-f256-496d-a8a2-5290f1f682d6.png)

**7. Tambahkan File ke Repository**

Untuk bisa menambahkan file ke repository GitHub, Anda perlu menerapkan langkah-langkah di bawah ini:

•	Buat file di folder yang sudah dibuat (Test Git). Contohnya, di sini kami membuat file index.php

•	Buka GitBash lalu masukkan perintah berikut:

$ git add index.php

Perintah tersebut tidak akan menghasilkan output apa pun.

**8. Buat Commit**
Selanjutnya, Anda perlu membuat Commit. Commit berfungsi untuk menambahkan update file serta komentar. 
Jadi setiap kontributor bisa memberikan konfirmasi update file di proyek yang sedang dikerjakan. 
Masukkan perintah berikut untuk membuat Commit:

$ git commit -m "first commit"

Pada tutorial ini saya membuat first commit sebagai Commit pertama saya. 
Kalian bebas membuat membuat nama Commit apa saja.

![Jepretan Layar 2021-10-21 pada 02 03 36](https://user-images.githubusercontent.com/92860030/138176210-51d1a9d1-0bc0-4598-972e-c4e08d0b14b3.png)

**9. Remote Repository Github**
Remote repository berfungsi untuk mengupload file yang telah kita buat sebelumnya di local disk. 
Masukkan perintah berikut ini untuk melakukan remote repository:

$ git branch -M main

$ git remote origin https://github.com/UserNameGit/NamaRepository

Perintah di atas tidak akan menghasilkan output apa pun.

**10. Push ke GitHub**
Langkah terakhir adalah push ke GitHub Push ini berfungsi untuk mengupload hasil akhir dari langkah-langkah di atas. 
Masukkan perintah berikut untuk melakukan push ke GitHub:

git push -f origin main

Anda perlu login untuk melanjutkan proses push ke GitHub. 
Jika proses login berhasil, akan muncul tampilan Command Prompt seperti di bawah:

![Jepretan Layar 2021-10-21 pada 03 24 59](https://user-images.githubusercontent.com/92860030/138176632-e9d3c1dd-2c9f-4dc1-9e83-83b9fffafb8b.png)

**11. Cek File**
Setelah itu, cek repository yang telah kalian buat. 
Kalian akan mendapati file-file yang telah ditambahkan sebelumnya. 
Pada tutorial ini kami menambahkan 1 file, yaitu index.php

![Jepretan Layar 2021-10-21 pada 04 46 49](https://user-images.githubusercontent.com/92860030/138177091-8274989a-bf18-4b16-a7d9-fec22b72c574.png)


