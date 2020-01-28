Sebagai seorang developer kita mungkin tidak asing dengan kata open source. banyak proyek open source yang tak sadar mungkin telah kita gunakan di kehidupan sehari hari kita sebagai manusia maupun sebagai developer . sebagai contohnya android, linux , framework codeigniter, react, laravel dan sebagainya. Tanpa kita sadar sebenernya industri IT saat ini sangat terpengaruh dengan proyek open source . di tulisan ini saya ingin mengajak teman teman belajar untuk berkontribusi ke ekosistem open source di event hacktoberfest 2019

## Apa Itu Hacktoberfest ?

[**Hacktoberfest](https://hacktoberfest.digitalocean.com)** adalah acara tahunan yang bertujuan untuk mendorong berkontribusi kedalam ekosistem *open source* . acara ini bebas untuk siapa saja , baik untuk pemula hingga professional sekalipun , berlangsung mulai dari tanggal 1 oktober hingga 31 oktober . acara tahun ini di jalankan oleh digital ocean , github dan dev.to . target dari acara ini adalah peserta dapat melakukan **4 pull request** di antara tanggal 1 hingga 31 oktober 2019.

![Hacktoberfest 2019 by digitalocean & dev.to](https://cdn-images-1.medium.com/max/4098/1*IFLgp1jCqGNWq7WCE3rICg.png)*Hacktoberfest 2019 by digitalocean & dev.to*

## Apa Benefit Mengikuti Hacktoberfest 2019?

Ada banyak hal yang bisa kamu dapetin apabila kamu mengikuti acara ini , antara lain :

1. Mendapatkan Swag (T-shirt & sticker) dari hacktoberfest (50.000 contributor pertama)

2. Memahami cara berkontribusi ke ekosistem open source

3. Memahami workflow dari ekosistem opensource

dan yang lainya.

## Bagaimana cara mengikuti hacktoberfest ?

1. **Buat akun github**
Pertama tama pastikan kamu memiliki akun github.com, karena nantinya kita akan melakukan kontribusi di ekosistem opensource yang ada di github

![akun github](https://cdn-images-1.medium.com/max/6720/1*i0oBRu7JpTPKoFFbsxJ31w.png)*akun github*

**2. Daftar hacktoberfest 2019**
yang kedua teman-teman wajib mendaftar di website resmi hacktoberfest2019 dengan menggunakan akun github

[https://hacktoberfest.digitalocean.com/](https://hacktoberfest.digitalocean.com/)

![](https://cdn-images-1.medium.com/max/6720/1*el0hw_ZYIk_Aq4sApqMXEQ.png)

**3.Pilih issue**
Pilih issue apa saja yang ada di github. kita bisa menggunakan label hacktoberfest untuk [mencarinya](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+archived%3Afalse+label%3Ahacktoberfest)

![list issue dengan label hacktoberfest](https://cdn-images-1.medium.com/max/3508/1*HlgGBUD8kFX5M3OePWtQ2w.png)*list issue dengan label hacktoberfest*

nah karena teman teman mungkin agak kesulitan mencari issue yang tempat disini saya sudah menyediakan 1 project yang dibuat untuk hacktoberfest

## **Animoji**

Animoji adalah aplikasi SPA berbasis vueJS yang bertujuan untuk menjelaskan anime dengan emoji , teman-teman dapat mengakses project ini di [**Github](https://github.com/2pai-dev/animoji)**

![[animoji](https://animoji.netlify.com)](https://cdn-images-1.medium.com/max/5244/1*4s1ROibI4377DLlGSLusYg.png)*[animoji](https://animoji.netlify.com)*

Cara berkontribusi di animoji

1. **fork repository animoji**

![fork repository](https://cdn-images-1.medium.com/max/5680/1*a_rd6fedzeVPSkR5aqmFTg.png)*fork repository*

**2.clone repository**
clone repository yang telah di fork tadi

    # $user is your github user
    git clone [https://github.com/$user/animoji](https://github.com/$user/animoji)

**3.Menambah Remote upstream**
tambahkan remote upstream dengan command

    git remote add upstream [https://github.com/2pai-dev/animoji](https://github.com/2pai-dev/animoji)

**4.Buat branch dan checkout**
buat branch baru dan checkout ke branch tersebut, semisal sword-art-online

    git branch sword-art-online 
    git checkout sword-art-online

**5. Menambahkan anime di list anime**
edit file src/store/listAnime.js dan tambahkan object baru sesuai format yang sudah ada , isi object tersebut dengan anime yang teman teman ingin masukan

![src/store/listAnime.js](https://cdn-images-1.medium.com/max/4560/1*4_RuSuEVMTi00ObdcRtrnA.png)*src/store/listAnime.js*

**6. git add & commit**

setelah melakukan pengeditan, lakukan command git add dan commit

    git add src/store/listAnime.js
    git commit -m ‘ add overlord anime ‘

**7. lakukan sync dengan upstream kemudian push**

    git fetch upstream
    git rebase upstream/master
    git push -f origin sword-art-online

**8. Lakukan pull request**

* buka repository hasil fork kamu di [https://github.com/$user/a](https://github.com/$user/kubernetes)nimoji

* klik tombol Compare & Pull Request button

* setelah itu buat masukan judul pull request & template pull request yang ada di repository

![pull request template](https://cdn-images-1.medium.com/max/3880/1*A7Mw1gGB41Z9SfcbAFNGrQ.png)*pull request template*

setelah itu tunggu hingga pull request tersebut di approve

## Kesimpulan

Semoga dari tulisan ini teman teman dapat melakukan kotribusi pertama ke ekosistem open source . dan juga semoga dari acara hacktoberfest ini dapat memantik semangat teman teman dalam belajar dan berkontribusi ke ekosistem open source.
