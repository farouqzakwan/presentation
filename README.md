# Tutorial github 

Pertama sekali apa yang anda perlukan adalah sebuah akaun github dan [git for windows](https://msysgit.github.io/), jika sekiranya anda menggunakan windows.

Kemudian anda digalakkan untuk mengikuti tutorial di 
[youtube](https://www.youtube.com/watch?v=_tN0T7jYn0A) untuk proses configuration. Sekiranya anda mengikuti video tutorial tersebut, anda tidak perlulah berulangkali memasukkan password anda.

Sekarang saya mengandaikan anda telah mempunyai akaun github dan telah mengikuti video tutorial di pautan yang tertera diatas.


##1) Hasilkan Repository baru dan folder projek

Untuk menghasilkan repository baru di github amatlah mudah..

Anda hanya perlu klik pada butang tambah dan pilih `new repository` untuk hasilkan _repo_ baru. Namakan repository anda , kemudian klik butang hijau "`create repository`":-


![new repo](https://github.com/farouqzakwan/presentation/blob/master/screenshot/new%20repo.PNG) 


![ create new repo](https://github.com/farouqzakwan/presentation/blob/master/screenshot/create%20new%20repo.PNG) 

Dalam gambar di atas, saya namakan repository saya yourRepoName. Memandangkan saya telah sedia ada mempunyai sebuah repository yang kosong, saya akan menggunakan repositori "presentation" untuk tutorial ini.

Kemudian hasilkan sebuah folder yang anda akan gunakan untuk projek anda..


Saya telah menghasilkan sebuah folder baru di desktop saya dan saya namakan ia sebagai "tutorial" dan di dalam folder tersebut saya hasilkan sebuah lagi folder "screenshot". Folder *screenshot* adalah bertujuan untuk menyimpan semua gambar yang diperlukan dalam tutorial ini.


##2) Jalankan perisian Git Bash

Sekarang jalankan perisian Git Bash anda dan tukar direktori ke direktori folder projek anda.Cara yang saya gunakan ialah, saya membuka folder **"tutorial"** kemudian tekan butang kanan tetikus dan saya pilih `git bash here`.

Bagi saya cara begini lebih menyenangkan kerana saya tidak perlu untuk menaip alamat direktori yang panjang.

##3) hasilkan file / code

Di dalam folder tutorial saya akan hasilkan sebuah file "**farouq.txt**" dan isi kandungannya adalah:-

```
hai saya farouq
```
![farouq txt](https://github.com/farouqzakwan/presentation/blob/master/screenshot/create%20farouq%20txt.PNG)


Tujuan saya hasilkan sebuah fail `text` dan mempunyai kandungan yang amat ringkas adalah supaya memudahkan anda membuat perbandingan setelah kandungan file ini di ubah nanti.

##4) git init

Di dalam perisian git bash anda, taip:-

```Batchfile
$ git init
```

Arahan ini bermaksud anda sedia menjadikan direktori dan subdirektori yang anda berada sekarang sebagai sebuah repositori.

![git init](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20init.PNG)

##5) git add

Arahan seterusnya adalah:-

```Shell
$ git add .
```

atau 

```Shell
$ git add farouq.txt
```

`git add` merupakan arahan untuk anda meletakkan file dan kod anda dalam keadaan _staging_ atau dalam erti kata lain bersedia sebelum anda `commit` kod anda.


Perbezaan kedua-dua arahan di atas ialah, arahan pertama meletakkan semua file yang belum anda jejaki/rekod(fail baru) atau fail yang telah di ubah dalam keadaan sedia untuk di `commit` manakala arahan kedua lebih bersifat memilih fail-fail tertentu sahaja.

![git add](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20add%201.PNG)

Dalam gambar di atas, terdapat dua baris perkataan yang berwarna merah. Ini bermaksud terdapat dua fail yang belum git jejak atau direkod perubahannya.

##6) git status

```Shell
$ git status
```

Arahan git status di gunakan untuk memeriksa status-status fail anda.

Setelah anda menaip arahan ini, anda akan dipaparkan status-status fail anda sama ada terdapat fail yang diubah (berwarna merah), sedia untuk di `commit` (berwarna hijau), konflik (berwarna merah), fail yang telah di buang (berwarna merah), atau direktori yang bersih.

##7) git commit

```
$ git commit -m "ruang tulis komen"
```

![git commit](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20commit%201.PNG)

Arahan ini digunakan setelah anda meletakkan file dan `kod` anda dalam keadaan sedia dan anda berpuas hati dengan hasil kerja anda. Disinilah poin-poin atau titik rujukan yang akan disimpan oleh git. Github membenarkan anda kembali kepada titik-titik rujukan ini sekiranya `kod-kod` anda selepas ini bermasalah atau anda membangunkan dua atau tiga versi yang berbeza. 

##8) git log

Arahan:-
```
$ git log
```

![log commit](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20log%201.PNG)

akan memaparkan log-log commit dan message anda.


##9) file yang diubah

Seterusnya saya akan mengubah kandungan `farouq.txt` dan menambah beberapa image ke dalam folder screenshot

kandungan baru dalam `farouq.txt` ialah:-

```
nama : farouq zakwan
umur : 23 (2015)
```

![ubah kandungan](https://github.com/farouqzakwan/presentation/blob/master/screenshot/change%20farouq%20txt.PNG)

Setelah melakukan perubahan apa yang perlu di buat ialah mengulangi arahan git add dan git commit..

![add image](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20add%203.PNG)

![commit file](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20commit%202.PNG)

##10) push to github

Jika anda masih ingat lagi, di awal tutorial ini saya telah mengajar bagaimana untuk menghasilkan sebuah repository baharu di github dan saya menyatakan yang saya akan  menggunakan *repository* *presentation* untuk tutorial ini. Sehingga sekarang saya masih lagi belum menulis bagaimana untuk menggunakannya.

Terdapat arahan yang perlu anda taip sebelum anda boleh push code anda ke repository github.

```
$ git remote add origin https://github.com/farouqzakwan/presentation.git
```

Setiap kali anda ingin push code anda ke repository ini,anda perlu menaip:-

```
$ git push -u origin master
```

##11) Lain-lain

Sehingga saat tutorial ini, banyak lagi perkara yang belum di bincangkan tentang cara penggunaan github. 
Antara perkara tersebut adalah bagaimana menggunakan github untuk kerjasama kumpulan,menulis README.md dalam format markdown.report an issue.kembali ke snapshot commit yang lepas.

Oleh itu saya amat mengharapkan anda dapat menambah baik tutorial ini dari semasa ke semasa.

- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed