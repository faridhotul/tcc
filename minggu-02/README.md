# PRAKTIKUM TEKNOLOGI CLOUD - PERTEMUAN 2

## NAMA : FARIDHOTUL KHASANAH / 175410026
## PRAKTIK KONFIGURASI GIT

1. Buka gitbash pada folder yang sudah di clone.
2. Ketikkan code berikut diisikan dengan username yang sama dengan saat mendaftar ke git.
   
   `$ git config --global user.name "faridhotul"`

    ![username](01.png)

3. Ketikkan code berikut, isikan email yang digunakan saat mendaftar git. 
   
   `$ git config --global user.email faridhotul.khasanah@gmail.com`

   ![email](02.png)

4. Untuk melihat konfigurasi, ketikkan :
   `$ git config --list`
   
   ![konfigurasi](03.png)
   
   
## PRAKTIK MENGELOLA REPO SENDIRI DI ACCOUNT SENDIRI
### 1. Membuat Repo

Langkah-langkahnya :

1.1 Klik tanda + pada bagian atas setelah login, pilih New repository

![repository](04.png)

1.2 Isikan nama, keterangan, serta lisensi. Jika dikehendaki, bisa membuat repo Private

![create](05.png)

1.3 Kemudian "Create Repository"

![create repository](06.png)

Bisa mengakses url disini : https://github.com/faridhotul/prakminggu2


### 2. Clone Repository

2.1 Clone repository dengan cara copy terlebih dahulu url untuk melakukan clone. Klik pada tombol _**Clone or Download > copy url**_

![gambar 07](07.png)

2.2 Setelah dicopy kan, silahkan masuk kedalam folder lokal untuk meng-clone project. Kemudian lakukan _**Klik Kanan > Git bash here**_

![gambar 08](08.png)

2.3 Kemudian ketikkan perintah 

`$ git clone https://github.com/faridhotul/prakminggu2.git`

![gambar 09](09.png)

2.4 Maka folder kosong yang sudah kita berikan clone proyek akan berubah menjadi ada isinya, yaitu project dari git. 

![gambar 10](10.png)

### 3. Mengelola Repo

3.1 Mengubah Isi - Push Tanpa Branching dan Merging

Membuat sebuah file dan dipush kedalam repository. 

1. Melakukan change directory. 

`$ cd prakminggu2`

2. Setelah masuk kedalam direktori tersebut, saya membuat file dengan nama README.md

`$ vim README.md`

Saya isikan "Halo my name is Faridhotul"

3. Melihat isi file. 

`$ cat README.md`

4. Melihat status direktori yang sekarang dijalankan.

`$ git status`

![gambar 15](15.png)

5. Menambahkan file kedalam direktori

`$ git add -A`

![gambar 16](16.png)

6. Commit file kedalam repository

`$ git commit -m "Add: README.md"`

![gambar 17](17.png)

7. Memasukkan file kedalam repository dengan istilah push kedalam origin master. 

`$ git push origin master`

![gambar 18](18.png)

Folder dalam local kita setelah membuat file README.md

![gambar 12](12.png)

Repository sebelum file dipush 

![gambar 13](13.png)

Repository setelah file dipush

![gambar 14](14.png)


3.2 Mengubah Isi dengan Branching and Merging

a. Buat branch untuk menampung perubahan-perubahan

`$ git checkout -b edit-readme-1`

![gambar 25](25.png)

Setelah membuat branch

![gambar 19](19.png)

Pada lokal kita akan terbentuk branch

![gambar 24](24.png)


b. Lakukan perubahan-perubahan

`$ vim README.md`

`$ cat README.md`

![gambar 26](26.png)

cek status branch

![gambar 27](27.png)

c. Add dan commit perubahan-perubahan tersebut ke branch

`$ git add -A`

`git commit -m "Add: README.md"`

![gambar 28](28.png)

![gambar 29](29.png)


d. Kembali ke repo master

`$ git checkout master`

![gambar 30](30.png)


e. Buat pull request di GitHub

`$ git push origin edit-readme-1`

![gambar 31](31.png)

Kirim pull request

![gambar 20](20.png)

Klik **Merge pull request"**

![gambar 21](21.png)

Klik **"confirm merge"**

![gambar 22](22.png)

Hasil setelah di pull request

![gambar 23](23.png)


f. Merge pull request di GitHub

`$ git merge edit-readme-1`

![gambar 32](32.png)

g. Merge branch untuk menampung perubahan-perubahan tersebut ke master.

`$ git branch -D edit-readme-1`

![gambar 33](33.png)

`$ git branch`

![gambar 34](34.png)

`$ git pull`

![gambar 35](35.png)

h. Selesai.


### 4. Sinkronisasi

`$ git pull`


### 5. Membatalkan Perubahan

a. Membuat branch untuk menampung perubahan-perubahan

`$ git checkout -b edit-readme-2`

![gambar 36](36.png)

b. Membuat file

`$ vim README.md`

![gambar 37](37.png)

`$ cat README.md`

![gambar 38](38.png)

c. Kembali ke master

`$ git checkout master`

![gambar 39](39.png)

d. Melihat file

`$ cat README.md`

![gambar 40](40.png)

e. Menghapus branch

`$ git branch -D edit-readme-2`

![gambar 41](41.png)

`$ git branch`

![gambar 42](42.png)

f. Melihat perubahan file walaupun brach sudah dihapus

`$ cat README.md`

![gambar 43](43.png)

g. Melakukan pembatalan perubahan

`$ git reset --hard`

![gambar 44](44.png)

h. Melihat file, perubahan tidak terjadi

`$ cat README.md`

![gambar 45](45.png)


### 6. Undo Commit Terakhir
