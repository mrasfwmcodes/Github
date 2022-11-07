# Github
what i learned with github


### `git clone` 
membuat salinan lokal dari proyek yang sudah ada dari jarak jauh. Klon mencakup semua file proyek, riwayat, dan cabang.

```
git clone https://github.com/mrasfwmcodes/tester.git
```

### `git init`
menginisialisasi repositori Git baru dan mulai melacak direktori yang ada. Itu menambahkan subfolder tersembunyi di dalam direktori yang ada yang menampung struktur data internal yang diperlukan untuk kontrol versi.
```
git init
```
### `git add`
tahapan sebuah perubahan. Git melacak perubahan pada basis kode pengembang, tetapi perlu untuk mengatur dan mengambil snapshot dari perubahan untuk memasukkannya ke dalam riwayat proyek. Perintah ini melakukan pementasan, bagian pertama dari proses dua langkah itu. Setiap perubahan yang dipentaskan akan menjadi bagian dari snapshot berikutnya dan bagian dari sejarah proyek. Pementasan dan komitmen secara terpisah memberi pengembang kendali penuh atas riwayat proyek mereka tanpa mengubah cara mereka membuat kode dan bekerja.
```
git add file1.md file2.md
```

### `git commit`
menyimpan snapshot ke riwayat proyek dan menyelesaikan proses pelacakan perubahan. Singkatnya, komit berfungsi seperti mengambil foto. Apa pun yang telah dipentaskan dengan git add akan menjadi bagian dari snapshot dengan `git commit`
```
git commit -m "first comment"
```

### `git status`
menunjukkan status perubahan sebagai tidak terlacak, dimodifikasi, atau bertahap.
```
git status
```

### `git branch`
menunjukkan cabang yang sedang dikerjakan secara lokal.
```
git branch
```
mengganti cabang ke main
```
git branch -M main
```
> bila terjadi seperti ini
```
$ git status
On branch master
Your branch is based on 'origin/master', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

nothing to commit, working tree clean
```
tinggal di ikuti sajja. itu terjadi karena hulu atau kepala cabang tidak ada
```
git branch --unset-upstream
```

### `git remote`
```
git remote
```
berikan jalur untuk repositori yang Anda buat di github
```
git remote add origin https://github.com/mrasfwmcodes/tester.git
```

### `git merge`
menggabungkan garis pembangunan bersama-sama. Perintah ini biasanya digunakan untuk menggabungkan perubahan yang dibuat pada dua cabang yang berbeda. Misalnya, pengembang akan menggabungkan ketika mereka ingin menggabungkan perubahan dari cabang fitur ke cabang utama untuk penyebaran.


### `git pull`
memperbarui jalur pengembangan lokal dengan pembaruan dari mitra jarak jauhnya. Pengembang menggunakan perintah ini jika rekan satu tim telah membuat komitmen ke cabang pada jarak jauh, dan mereka ingin mencerminkan perubahan tersebut di lingkungan lokal mereka.

### `git push`
memperbarui repositori jarak jauh dengan komit apa pun yang dibuat secara lokal ke cabang.
