“#Latihan 1”

 Menambahkan Global Config
 
• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

• konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

• Config Global Repository

    $ git config --global user.name “nama_user”
 
    $ git config --global user.email “nama_user”
 
 ![1](https://user-images.githubusercontent.com/44828491/66741850-95fbdc80-eea0-11e9-870a-e84b4a6ae9c3.png)

 Membuat Reposiory Local
 
• Buka direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer)

• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

![2](https://user-images.githubusercontent.com/44828491/66741976-dc513b80-eea0-11e9-9114-694e7f08c749.png)

• Buat direktory project praktikum pertama dengan nama latihan1

    $ mkdir latihan1
 
    $ cd latihan1
    
![3](https://user-images.githubusercontent.com/44828491/66742025-f25efc00-eea0-11e9-8985-f1199f65e8b1.png)

• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd
 (change directory)
 
• direktory aktif menjadi: d:\labs_pemrograman1\latihan1

![4](https://user-images.githubusercontent.com/44828491/66742079-0b67ad00-eea1-11e9-9720-b347750208a8.png)

 Membuat Reposiory Local
 
• Jalankan perintah git init, untuk membuat repository local.

    $ git init

![5](https://user-images.githubusercontent.com/44828491/66742202-597cb080-eea1-11e9-85bc-fb3ba405dcec.png)

• Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git

• Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

 Menambahkan File baru pada repository
 
• Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

• disini kita akan coba buat satu file bernama README.md (text file)

    $ echo ”#Latihan 1” >> README.md
    
![6](https://user-images.githubusercontent.com/44828491/66742316-947ee400-eea1-11e9-84dd-a5a79861a35f.png)

• File README.md berhasil dibuat.

 Menambahkan File baru pada repository
 
• Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

    $ git add README.md
    
    

• File README.md berhasil ditambahkan.

 Commit (Menyimpan perubahan ke database)
 
• Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar
  commit”
  
    $ git commit -m “File pertama saya”
    
![8](https://user-images.githubusercontent.com/44828491/66742501-f93a3e80-eea1-11e9-9835-765e6ee5cd73.png)

• Perubahan berhasil disimpan.

 Membuat repository server
 
• Server reopsitory yang akan kita gunakan adalah http://github.com

• Anda harus membuat akun terlebih dahulu.

• Pada laman github, klik tombol start a project, atau

• Dari menu (icon +) klik New Repository

![9](https://user-images.githubusercontent.com/44828491/66742597-37376280-eea2-11e9-9d27-c4f1d0e5bf33.png)

 Membuat repository server
 
• Isi nama repositorynya, misal: labpy1.

• lalu klik tombol Create repository

![10](https://user-images.githubusercontent.com/44828491/66742636-4dddb980-eea2-11e9-8e5a-1df625100f2c.png)
 
 Menambahkan Remote Repository

• Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local
  repository, sehingga dapat diakses oleh banyak user.
  
• Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

    $ git remote add origin https://github.com/abuazzam/labpy1.git
     
![11](https://user-images.githubusercontent.com/44828491/66742742-9006fb00-eea2-11e9-8f3f-822cf2471e33.png)   

 Push (Mengirim perubahan ke server)

• Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

    $ git push -u origin master
    
 ![12](https://user-images.githubusercontent.com/44828491/66742886-e4aa7600-eea2-11e9-9133-b44589134878.png)

• Perintah ini akan meminta memasukkan username dan password pada akun github.com

 Melihat hasilnya pada server repository
 
• Buka laman github.com, arahkan pada repositorinya.

• Maka perubahan akan terlihat pada laman tersebut.

 Clone Repository
 
• Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai
  dengan nama repositorynya (working directory).
  
• Untuk melakukan cloning, gunakan perintah git clone [url]


