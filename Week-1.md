# Week 1
## A. _Unit Command Line_
- CLI merupakan akronim dari Command Line Interface. Dengan program ini, user bisa mengetikkan perintah dalam bentuk teks dan memberikan instruksi pada komputer untuk mengerjakan tugas tertentu.
- Saat kita menyebut "command line" atau "command line interface", sebenarnya yang dimaksud adalah shell yang berbasis teks. Shell ini adalah program yang menerima perintah, kemudian meneruskan perintah tersebut ke system untuk dieksekusi. 
- Contoh dari CLI, yaitu : bash dan cmd.exe
- Filesystem mengatur bagaimana data disimpan di dalam sebuah system
- Sistem operasi Windows & Unix-like menyusun file dan direktori menggunakan struktur yang bentuknya mirip tree
- **Command untuk navigasi :**
1. pwd (Print working directory) : Command untuk melihat current working directory
2. ls (lists) : Command untuk melihat isi file yang ada di sebuah direktori
3. cd <direktori> (change directory) : Command untuk berpindah direktori.
- **Command untuk membuat Files dan Direktori :**
1. touch : Command untuk membuat sebuah file
2. mkdir : Command untuk membuat sebuah direktori
- **Command untuk Melihat isi files :**
1. head : Command untuk melihat beberapa line awal dari sebuah file text
2. tail : Command untuk melihat beberapa line akhir dari sebuah file text
3. cat : Command untuk melihat isi sebuah file
- **Command untuk menyalin, memindahkan, dan menghapus files & directory :**
1. cp (copy) : Command untuk mengcopy files atau directory (cp -R untuk menyalin direktori)
2. mv (move) : Command untuk memindahkan files atau directory (mv -R untuk memindahkan direktori) serta dapat digunakan untuk rename
3. rm (remove) : Command untuk menghapus file atau directory (rm -R atau rm -d untuk menghapus direktori)

## B. _GIT & GITHUB_
- GIT merupakan tools untuk programmer dan sebagai version control system
- Tugas dari version control system yaitu mencatat setiap perubahan pada File (termasuk code yang kita buat) pada suatu proyek baik dikerjakan secara individu maupun tim.
- Git adalah aplikasi yang dapat melacak setiap perubahan yang terjadi pada suatu folder atau file. Git digunakan sebagai tempat penyimpanan file pemrograman mereka, karena lebih efektif.
- Tujuan dari penggunaan Git dan Github yaitu agar kita bisa berkolaborasi mengerjakan proyek yang sama tanpa harus repot copy dan paste folder aplikasi yang terupdate
- Git dan GitHub menangani commands secara berbeda. Developer yang menggunakan Git dapat menggunakan command-line tool, yaitu pengubah kode dan dapat digabungkan menuju perangkat lokal. Sedangkan, GitHub menyediakan interface grafis berbasis cloud sebagai tempat untuk melakukan seluruh tugas.
- **Setup Awal Git :**
1. git config global user.email rafipersonalporto@gmail.com (email yang digunakan harus sama dengan Github)
2. git config global user.name "Rafi"
3. git config --list untuk melihat hasil konfigurasi
4. git init (dilakukan pada folder yang dibuat) untuk membuka repository
5. git status untuk mengecek perubahan pada Git
6. git add . untuk menambahkan file baru pada Git
7. git commit -m "Pesan Commit" untuk menyimpan perubahan pada Git
8. git push -u origin master / main untuk mengirim file pada remote repository
9. git clone untuk mengambil repository lokal

## C. _HTML_
- HTML (Hypertext Markup Language) berfungsi untuk membuat kerangka dari sebuah website dan digunakan untuk menampilkan konten pada browser
- HTML memiliki sifat statis dan bukan merupakan bahasa pemrograman
- Tools yang dibutuhkan : Browser dan Code Editor
- Visual Studio Code merupakan salah satu code editor yang dikembangkan oleh Microsoft
- Keunggulan dari Visual Studio Code, yaitu dapat digunakan di Windows, Mac, dan juga Linux.
- HTML Structure : 
```sh
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Belajar HTML</title>
    <link rel="stylesheet" href="test.css" />
  </head>
  <body></body>
</html>
```
- HTML Element : Opening tag, Content, dan Closing tag
- HTML attribute merupakan properties dari HTML Element (id, class)
- HTML Comment berfungsi untuk memberikan penjelasan line dari code yang kita kerjakan
- Terdapat Single tag dan Double tag pada HTML
- Untuk menampilkan file HTML secara live kita bisa menginstall extension bernama "Live Server" pada Visual Studio Code
- Semantic HTML yaitu menggunakan elemen HTML sesuai kebutuhan konten seperti header, footer, dan nav
- Contoh penggunaan Semantic HTML tag : 
```sh
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Belajar HTML</title>
    <link rel="stylesheet" href="test.css" />
  </head>
  <body>
    <nav>
      <ul>
        <li><a href="">Nama</a></li>
        <li><a href="">Umur</a></li>
        <li><a href="">About</a></li>
      </ul>
    </nav>
    <script src="script.js"></script>
  </body>
</html>
```
- Kita bisa menggunakan **Netlify** untuk melakukan deploy terhadap HTML yang sudah kita buat agar bisa diakses oleh semua orang

## D. _CSS_
- CSS (Cascading Style Sheets) berfungsi untuk mendesain sebuah halaman website.
- kita bisa mengubah warna, menggunakan font custom, editing text format, dan mengatur tata letak dengan menggunakan CSS
- Struktur CSS, yaitu :
```sh
.ElementHTML {
  property: value;
}
```
- CSS Comment memiliki fungsi yang sama dengan HTML Comment yaitu untuk memberikan penjelasan line dari code yang kita kerjakan (/* */)
- Terdapat 3 cara penggunaan CSS :
1. Inline Style : menambahkan CSS pada attribute element HTML
2. Internal Style : menggunakan tag style di bagian head
3, External Style : menggunakan file css terpisah dengan html
- . / titik : merupakan selector untuk tag html yang memiliki properti class
- Contoh properti pada CSS : color, background-color
- Cara menghubungkan / mengakses file CSS pada HTML
```sh
<link rel="stylesheet" href="contoh.css" />
```
- CSS - Tag Name : Kita bisa menggunakan Tag Elemen HTML secara langsung pada CSS dan elemen tersebut akan bersifat global (mempengaruhi seluruh Tag Elemen HTML yang ada pada file tersebut)
```sh
h1 {
  color: red;
}
```
- CSS - Class Name : Kita bisa menggunakan attribute class pada elemen HTML lalu memanggil nama class tersebut pada CSS (class yang sama akan mempunyai styling yang sama saat digunakan pada CSS)
```sh
.contoh {
  color: red;
}
```
- CSS - ID Name : Berbeda dengan Class Name. ID Name bersifat unik artinya hanya ada 1 nama ID pada 1 element HTML.
```sh
#navigation {
  display: inline;
}
```
- Perbedaan antara ID dan Class adalah ID Name digunakan  jika hanya ada 1 elemen pada file/halaman HTML seperti header dan footer. Sedangkan Class Name digunakan jika ada beberapa element HTML yang memiliki styling/desain yang sama.
- Nested element : Parent and Child (konsep pada css)
- Multiple selector digunakan agar codingan kita semakin efisien dan tidak berulang ulang
```sh
Sebelum :
h1 {
    color: brown;
    font-family: 'Courier New', Courier, monospace;
}

p {
    font-family: 'Courier New', Courier, monospace;
}

Sesudah ;
h1 {
  color: brown;
}

h1, p {
  font-family: "Courier New", Courier, monospace;
}
```
**FLEXBOX**
- Flexbox merupakan cara untuk mengatur layout serta dapat menyesuaikan layout secara otomatis.
- Flexbox memiliki 1 parent dan beberapa child
- flex-direction digunakan untuk mengatur letak item child.
- flex-wrap digunakan untuk membatasi jumlah item children dalam 1 line
- flex-flow digunakan sebagai shortcut untuk set up flex-direction dan flex-wrap bersamaan.
- Properti order berfungsi untuk ordering item mana yang ingin kita atur posisinya berdasarkan urutan order.
- justify-content digunakan untuk mengatur tata letak dan space antar item child secara horizontal 
- align-items digunakan untuk mengatur align dari item child secara vertikal 
- align-self digunakan untuk mengatur align item pada masing-masing item.
- flex-grow dapat mengatur size suatu item child pada flexbox.
- flex-shrink adalah properti yang membuat size suatu item child mengecil secara relatif terhadap item child lainnya.
- flex-basis adalah properti yang sama fungsinya seperti width yaitu mengatur width dari setiap item child

## E. _Algoritma & Pseudocode_
- Algoritma merupakan proses menyelsaikan suatu masalah yang dilakukan secara logis dan sistematis
- Belajar algoritma sama dengan mengingat kembali alur berfikir yang terstruktur
- Mempelajari algoritma merupakan hal penting di dalam dunia programming
- Ciri-ciri algoritma : Input, Output, Definiteness (pasti), Finiteness (memiliki batas), dan Effectiveness (tepat dan efisien)
- Perbedaan antara algoritma dan data struktur yaitu data struktur berfungsi untuk mengatur / mengelola suatu data, sedangkan algoritma berfungsi menyelesaikan masalah menggunakan data-data tersebut
- Contoh algoritma secara deskriptif :
```sh
1. Apakah kamu haus?
2. Jika ya, minum lalu ke no 4
3. Jika tidak, tidak perlu minum lalu ke no 4
4. Selesai
```
- Pseudocode merupakan penulisan algoritma sebelum kita implementasikan ke bahasa pemograman tertentu.
- Panduan menulis pseudocode :
```sh
1. Menggunakan huruf besar pada kata kunci. 
2. 1 statement terdiri dari 1 baris 
3. Gunakan indentasi
4. Spesifik dan simpel
```
- Contoh pseudocode :
```sh
BEGIN
NUMBER s1, s2, sum
OUTPUT("Input number1:")
INPUT s1
OUTPUT("Input number2:") 
INPUT s2
sum=s1+s2
OUTPUT sum
END
```
- Jenis-jenis pseudocode :
1. Procedural : Berpikir secara runtut
2. Conditional : Percabangan kasus (if else)
3. Looping : Proses yang sama berulang-ulang (for, while)
4. Recursive : Algoritma yang memanggil method / function

## F. _Javascript Dasar_
- Javascript adalah bahasa pemograman yang sangat powerful yang digunakan untuk logic pada sebuah website
- Javascript juga dapat membuat website menjadi interaktif dan dinamis
- Contoh syntax pada javascript : Alert(), Confirm(), dan Prompt()
- Console log dapat digunakan untuk melakukan debugging (mengetahui error pada code) pada pemograman web dan cek logic pemograman web yang kita kembangkan
- Tipe data merupakan klasifikasi yang kita berikan untuk berbagai macam data
- 6 tipe data fundamental pada Javascript :
1. number : tipe data yang mengandung semua angka termasuk angka desimal.
2. string : grup karakter yang ada pada keyboard laptop/PC kita yaitu letters (huruf), number (angka), spaces (spasi), symbol, dan lainnya
3. boolean : tipe data yang hanya mempunyai 2 buah nilai yaitu TRUE dan FALSE
4. null : tipe data yang diartikan bahwa sebuah variable/data tidak memiliki nilai.
5. undefined : tipe data yang merepresentasikan varibel/data yang tidak memiliki nilai.
6. object : koleksi data yang saling berhubungan (related). Tipe data pbject dapat menyimpan data dengan tipe data apapun (number, string, boolean, dan lainnya)
- Variable merupakan tempat untuk menyimpan sebuah nilai
- 3 cara mendefinisikan variabel pada Javascript : 
1. var
2. let
3. const : variabel yang tidak dapat diubah nilainya
- Assignment operator (=) digunakan untuk menyimpan sebuah nilai pada variabel
- increment(++) atau decrement(--) untuk menambah atau mengurangi sebesar 1 nilai
- Arithmetic operator adalah operator yang melibatkan operasi matematika (Tambah (+), Kuramg (-), Perkalian (*), Pembagian (/), Modulus (%) )
- Comparison operator adalah operator yang membandingkan satu nilai dengan nilai lainnya yang memiliki hasil TRUE atau FALSE
- Simbol comparison operator :
1. Lebih kecil dari : <
2. Lebih besar dari: >
3. Lebih kecil atau sama dengan: <=
4. Lebih besar atau sama dengan: >=
5. Sama dengan: ===
6. Tidak sama dengan: !==
- Logical operator biasa digunakan untuk sebuah CONDITIONAL pada pemograman yang memiliki hasil TRUE atau FALSE
- Simbol dari Logical Operator adalah sebagai berikut:
1. AND operator : &&
2. OR operator: ||
3. NOT operator: !
- Conditional merupakan statement percabangan yang menggambarkan sebuah kondisi
- Beberapa contoh conditional : 
1. if statement
2. if else statement
3. Switch case conditional : digunakan ketika kondisi percabangan terlalu banyak
- Looping merupakan statement yang mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop tercapai
- Beberapa contoh Looping : 
1. For Loop : digunakan ketika mengetahui seberapa banyak nilai pasti untuk pengulangannya
2. While Loop : menjalankan instruksi pengulangan kondisi bernilai TRUE. Digunakan ketika tidak mengetahui jumlah pasti pengulangan
3. Do While Loop
- Nested loop : membuat looping didalam looping. 
