GIT REMOTE  

    1. Poin utama :
   
        A. Apa itu git remote?

            Git remote adalah cara untuk menghubungkan repositori lokal dengan repositori remote. Repositori remote adalah tempat di mana kode Anda disimpan dan dapat diakses oleh orang lain. Dalam penggunaan git, Anda akan menghubungkan repositori lokal Anda dengan repositori remote yang telah dibuat.

        B. Cara Kerja git remote

            1.Membuat Repository di GitHub:
                -Buka GitHub dan buat sebuah repository dengan nama, misalnya, “belajar-git”.
                -Repository ini akan menjadi tempat kita menyimpan kode proyek secara remote.

            2.Menambahkan Remote:
                -Sebelum kita dapat mengirim revisi ke repository remote, kita harus menambahkan remote terlebih dahulu.
                -Gunakan perintah berikut untuk menambahkan remote:
                    [git remote add github git@github.com:petanikode/belajar-git.git]
                        ->Di sini, github adalah nama remote, dan URL-nya adalah git@github.com:petanikode/belajar-git.git.
                        ->Catatan: Jika menggunakan HTTPS, kita akan diminta password setiap kali melakukan push. Jika menggunakan SSH, kita tidak perlu memasukkan password, tetapi kita harus mengonfigurasi SSH Key terlebih dahulu.

            3.Melihat Remote yang Sudah Ditambahkan:
                -Ketik perintah berikut untuk melihat remote apa saja yang sudah ditambahkan:
                    [git remote -v]

            4.Mengirim Revisi ke Remote Repository:
                -Gunakan perintah git push untuk mengirim revisi ke repository remote:
                    [git push github master]
                        ->Di sini, github adalah nama remote, dan master adalah nama cabang tujuan.
                        ->Pastikan kita sudah melakukan beberapa revisi sebelum melakukan push:
                            [git add . ,git commit -m "menambahkan beberapa revisi"]

        C.apa itu git clone
            Git clone adalah perintah dalam Git yang digunakan untuk membuat salinan lengkap dari suatu repositori. Perintah ini meng-copy semua file, log, dan versi dari repositori asli ke direktori baru di komputer lokal pengguna1. Contoh sederhana penggunaan git clone adalah saat seorang developer ingin bekerja pada proyek yang sudah ada di GitHub.

    2.kesimpulan
        Git remote adalah fitur yang memungkinkan kita berinteraksi dengan repositori remote dari repositori lokal kita. Dalam pengembangan perangkat lunak, kita sering bekerja dengan repositori yang berada di server jarak jauh, seperti GitHub, GitLab, atau Bitbucket dan membuat kita lebih mudah untuk berkerja dalam tim
