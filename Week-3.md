# Week 3
## A. _Javascript Intermediate Array_
- Array merupakan tipe data list order yang dapat menyimpan tipe data apapun di dalamnya.
- Array dapat menyimpan tipe data String, Number, Boolean, dan lainnya.
- Contoh Array : 
```js
let makanan = ['ayam goreng', 'bebek goreng']
console.log(makanan)
// Output : [ 'ayam goreng', 'bebek goreng' ]
```
- Array didefinisikan menggunakan square brackets ([])
- Array pada javascript dihitung dari index data ke-0 (Data Pertama).
```js
let makanan = ['ayam goreng', 'bebek goreng']
// index ke - 0 = ayam goreng
// index ke - 1 = bebek goreng

console.log(makanan[0])
// Output : ayam goreng
```
- Kita dapat mengupdate data pada Array.
- Contoh : 
```js
let makanan = ['ayam goreng', 'bebek goreng']
makanan[0] = 'pisang goreng'
console.log(makanan)
// Output : [ 'pisang goreng', 'bebek goreng' ]
```
- Const tidak bisa melakukan update data. Namun pada Array kita dapat melakukan update konten nilai di dalam array (mutable), yang tidak bisa kita lakukan adalah mengubah array dengan array yang baru jika menggunakan const
- Array memiliki 5 properti, yaitu constructor, length, index, input, dan prototype.
- Properties adalah fitur yang sudah disediakan oleh Javascript untuk memudahkan developer.
- Length akan mengembalikan nilai dari jumlah panjang data suatu array.
- Contoh : 
```js
let makanan = ['ayam goreng', 'bebek goreng']
console.log(makanan.length)
// Output : 2
```
- Array memiliki method atau biasa disebut built-in methods yang memiliki arti javascript sudah memudahkan kita dengan menyediakan function/method umum yang bisa kita gunakan.
- Kita tidak perlu membuat function lagi jika method yang kita butuhkan sudah tersedia.
- Contoh array built-in : 
1. .push() : method untuk menambahkan item  array pada urutan yang paling akhir.
```js
let makanan = ['ayam goreng', 'bebek goreng']
makanan.push('pisang goreng')
console.log(makanan)
// Output : [ 'ayam goreng', 'bebek goreng', 'pisang goreng' ]
```
2. .pop() : method yang menghapus item array index terakhir.
```js
let makanan = ['ayam goreng', 'bebek goreng']
makanan.pop()
console.log(makanan)
// Output : [ 'ayam goreng' ]
```
3. .shift() : method untuk menghapus item Array pada index pertama.
```js
let makanan = ['ayam goreng', 'bebek goreng']
makanan.shift()
console.log(makanan)
// Output : [ 'bebek goreng' ]
```
4. .unshift() : method untuk menambahkan item Array pada index pertama.
```js
let makanan = ['ayam goreng', 'bebek goreng']
makanan.unshift('pisang goreng')
console.log(makanan)
// Output : [ 'pisang goreng', 'ayam goreng', 'bebek goreng' ]
```
5. .sort() : method untuk mengurutkan secara Ascending atau Descending Alphanumeric. 
```js
const number = [5, 3, 4, 2, 1]
number.sort()
console.log(number)
// Output : [ 1, 2, 3, 4, 5 ]
```
- Array memiliki built in methods untuk melakukan looping yaitu .map() dan .forEach().
- .forEach() : method untuk melakukan looping pada setiap elemen array.
```js
let makanan = ['ayam goreng', 'bebek goreng', 'pisang goreng']
makanan.forEach(element => {
    console.log(makanan)
})
// Output : "ayam goreng", "bebek goreng", "pisang goreng"
```
- .map() : melakukan perulangan/looping dengan membuat array baru.
```js
let number = [1, 2, 3 , 4, 5, 6]
let num = number.map(numb => {
    return numb * 2
})
console.log(num)
// Output : [ 2, 4, 6, 8, 10, 12 ]
```
- Perbedaannya yaitu .forEach tidak dapat membuat Array baru dari hasil operasi yang ada dalam looping.
- .forEach() digunakan jika hanya memerlukan looping untuk menampilkan saja atau menyimpan ke database.
- .map() digunakan jika akan melakukan operasi pada array seperti yang dapat mengubah nilai array sebelumnya.
## B. _Javascript Intermediate Multidimensional Array_
- Multidimensional Array bisa dianalogikan dengan array of array (array di dalam array).
- Contoh : 
```js
let orang = [["andi", "Cowok"], ["Putri", "Cewek"]]
console.log(orang)
// Output : [ [ 'andi', 'Cowok' ], [ 'Putri', 'Cewek' ] ]
```
- Sama seperti array satu dimensi, multidimensional array juga dapat menggunakan Property dan Method built-in Array.
## C. _Javascript Intermediate Object_
- Object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method). 
- Properti adalah data lengkap dari sebuah object.
- Method adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.
- Contoh tipe data : 
1. number
2. string
3. boolean
4. null
5. undefined
6. array
7. object
- Object dapat diassign kedalam sebuah variabel.
```js
let contoh = {}
// contoh adalah sebuah objek kosong

let orang = {
    nama: andi,
    umur: 20,
}
// objek orang dengan properti
```
- Di dalam object kita dapat menyimpan properti dengan tipe data apapun.
- Contoh mengakses objek serta properti objek : 
```js
let orang = {
    nama: "andi",
    umur: 20,
}
console.log(orang)
// Output : { nama: 'andi', umur: 20 }
```
- Kita juga bisa menggunakan bracket notation saat memanggil properti dari sebuah object.
```js
let orang = {
    nama: "andi",
    umur: 20,
}
console.log(orang['nama'])
// Output : 'andi'
```
- Kita dapat melakukan update pada variabel dengan tipe data Object.
- Object dapat mengupdate value dari key yang sudah tersedia serta dapat menambahkan key dan value baru.
- Contoh update data pada object : 
```js
let orang = {
    nama: "andi",
    umur: 20,
}
orang.nama = "randy"
console.log(orang)
// Output : { nama: 'randy', umur: 20 }
```
- Jika menggunakan constant pada variable object. Kita tidak bisa mengganti seluruh data object dengan object yang baru.
- Ketika membutuhkan untuk update seluruh data object gunakan ‘let’ pada saat deklarasi variabel.
- Kita dapat menghapus properti dari object menggunakan **delete** operator.
- Contoh : 
```js
let orang = {
    nama: "andi",
    umur: 20,
}
delete orang.umur
console.log(orang)
// Output : { nama: 'andi' }
```
- Jika value yang kita masukkan pada property berupa function maka akan disebut method.
- Console merupakan global javascript object, log() merupakan property yang berupa function dari object console, Sehingga kita memanggila dengan cara console.log().
```js
const contoh = {
    tanya: function() {
        return "kamu siapa ?"
    },
    
    jawab: function() {
        return "saya rafi"
    }
}
console.log(contoh.tanya())
console.log(contoh.jawab())
// Output : kamu siapa ? , saya rafi
```
- Nested Object : Object yang berasal dari turunan object lainnya.
- Kita dapat mengubah data yang ada pada object melalui sebuah function dan memasukkan object sebagai parameter function (pass by reference).
- Contoh : 
```js
let angka = {
    satu: 1,
    dua: 2
}

function ubah(num) {
    num.satu = 11
    num.dua = 22
}
ubah(angka)
console.log(angka)
// Output :  { satu: 11, dua: 22 } -> mengubah data object dengan function ubah
```
- Jika kita ingin menampilkan seluruh object properti, kita dapat menggunakan looping sehingga tidak perlu mengakses secara manual memanggil setiap propertinya.
- Contoh : 
```js
let angka = {
    satu: 1,
    dua: 2,
    tiga: 3,
    empat: 4
}

for(let data in angka) {
    console.log(angka[data])
}
// Output : 1, 2, 3, 4
```
- Object sama seperti Array yang bisa menyimpan banyak data (menggunakan array of object).
- Contoh : 
```js
let orang =[
    {nama: "rafi", umur: 19},
    {nama: "andi", umur: 20}
]
orang.forEach((listorang) => {
    console.log(listorang)
})
// Output : { nama: 'rafi', umur: 19 }, { nama: 'andi', umur: 20 }
```
## D. _Javascript Intermediate Recursive_
- Recursive merupakan function yang memanggil dirinya sendiri sampai kondisi tertentu.
- Recursive biasanya digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.
- Struktur : 
```js
function recursive() { 
    recursive()
}
```
- Ciri-ciri rekursif : 
1. Selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar.
2. Selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.
- Contoh : 
```js
function hitung(x, n) {
    if (n == 1) {
        return x
    } else {
        return x * hitung(x, n - 1)
    }
}
console.log(hitung(2, 3)) // Output : 8
```
- Contoh recursive dengan kondisi tertentu.
```js
function recursive() {
    if(condition){
        // stop calling it self

    } else {
        recursive();
    }
}
```
## E. _Javascript Intermediate Asynchronous_
- Asynchronous merupakan perintah di eksekusi yang tidak berdasarkan urutan kode, melainkan berdasarkan waktu proses. tidak bersifat blocking, asynchronous akan mengeksekusi perintah selanjutnya tanpa menunggu perintah sebelumnya selesai dijalankan.
- Contoh : 
```js
console.log('test')
setTimeout() => {
    console.log('contoh'), 100 // yang berarti perintah akan tertunda selama 100 ms
    console.log('contoh1')
}
// Output :
test
contoh1
contoh
```
```sh
Dapat disimpulkan bahwa hasil dari output asynchronous tidak urut sesuai dengan urutan kode, pengeksekusian contoh tertunda karena kita melakukan setTimeout() akan tetapi proses eksekusi contoh1 tetap berjalan tanpa harus menunggu contoh selesai. Hal ini menggambarkan cara kerja Asynchronous yaitu berdasarkan waktu proses.
```
- Sedangkan Synchronous berjalan berdasarkan urutan kode yang kita ketikkan.
- Race condition merupakan pertimbangan dalam penggunaan Asynchronous dan terjadi ketika ada satu perintah yang bergantung pada output eksekusi Asynchronous sebelumnya.

- callback merupakan sebuah function, perbedaan dengan function lainnya yaitu pada cara eksekusinya. callback di eksekusi dalam function lain melalui parameter.

```js
function main(param1,param2,callBack){ 
  console.log(param1, param2) 
  callBack()  
}

function myCallback(){ 
  console.log ('hello callback')
}

main(1,2,myCallback)
// Output :
//  1 2
//  hello callback
```
- Function dalam javascript adalah object atau sering disebut first-class object, yang memiliki arti :
1. Function bisa di jadikan parameter
2. Function dapat disimpan ke dalam variabel
3. Seperti object pada umumnya, function bisa memiliki property dan method
4. Function dapat mengembalikan value dalam bentuk function

- Callback dapat digunakan untuk proses synchronous dan asynchronous.
- Contoh implementasi : 
1. Injeksi atau modifikasi hasil eksekusi sebuah function
2. Event listener
3. Menangani proses asynchronous


- Promise merupakan sebuah fitur terbaru dari ES6.
- Terdapat 3 kemungkinan state ketika melakukan request asynchronous (contoh : Ajax), yaitu :
1. Pending ( sedang dalam proses )
2. Fulfilled ( berhasil )
3. Rejected ( gagal )

- Promise merupakan alternatif dari callback. agar membuat code lebih readable dan manajemen error yang lebih baik.

- Perbedaan antara callback dan promise :
1. Callback adalah function sedangkan promise adalah object.
2. Callback di kirim melalui parameter, sedangkan promise mengembalikan object
3. Callback digunakan untuk menghandle succes dan failure,sedangkan - promise tidak
4. Callback dapat digunakan untuk beberapa event sekaligus, sedangkan promise hanya untuk satu event
- Cara membuat promise yaitu cukup dengan memanggil constructor nya :
- Contoh :
```js
let contoh = new promise()
console.log(contoh)

// Output : promise {<pending>}
```

- Karena kita belum mengatur state Fullfilled dan Reject, maka kita gunakan salah satu listener :
1. resolve()
2. reject()
```js
let prom = new promise((resolve, reject) => {
    // salah satu dari 2 callback berikut
    // resolve ('berhasil')
    // reject (err('Janji dibatalkan'))
});

//untuk menggunakan promise diatas mari gunakan method then dan catch

prom.then((result) =>{
    console.log(result)
}.catch((error) =>{
    console.log(error)
}))
```
- Gambaran :
```sh
resolve() -----------> .then(result)
          (fulfilled)
reject()  -----------> .catch(error)
          (error)
```  
## F. _Javascript Intermediate Web Storage_
- Sebelum HTML5, data aplikasi harus disimpan dalam cookie, termasuk dalam setiap permintaan server. web storage termasuk lebih aman, dan sejumlah besar data dapat disimpan secara lokal, tanpa memengaruhi kinerja situs web.
- Tidak seperti cookie, batas penyimpanan jauh lebih besar (minimal 5MB) dan informasi tidak pernah ditransfer / dikirim ke server.
- Maksimum data yang dapat disimpan dalam cokies adalah 4Kb.
- Kekurangan cookies
  1. Setiap kita mengakses situs web, cookies juga kembali dikirim sehingga memperlambat aplikasi web kamu dengan mengirimkan data yang sama.
  2. Cookies disertakan pada setiap HTTP request, sehingga mengirimkan data yang tidak dienkripsi melalui internet, maka saat kita ingin menyimpan data dalam cookies kita harus mengenkripsinya terlebih dahulu.
  3. Cookies hanya dapat menyimpan data sebanyak 4KB.
  4. Cookies juga memiliki tanggal kadaluarsa. Tanggal ini telah ditentukan sehingga web browser bisa menghapus cookies jika tanggal sudah kadaluarsa atau tidak dibutuhkan.
- Penyimpanan web adalah per asal (per domain dan protokol). Semua halaman, dari satu asal, dapat menyimpan dan mengakses data yang sama.
- HTML Web Storage menyediakan dua objek untuk menyimpan data pada klien :
1. window.localStorage : menyimpan data tanpa tanggal kedaluwarsa.
2. window.sessionStorage : menyimpan data untuk satu sesi (data hilang saat tab browser ditutup).
- Sebelum menggunakan penyimpanan web, periksa dukungan browser untuk localStorage dan sessionStorage dengan : 
```js
if (typeof(Storage) !== "undefined") {
  // Code for localStorage/sessionStorage.
} else {
  // Sorry! No Web Storage support..
}
``` 
- Objek localStorage menyimpan data tanpa tanggal kedaluwarsa. Data tidak akan dihapus saat browser ditutup dan akan tersedia pada hari, minggu, atau tahun berikutnya.
- Contoh : 
```js
<!DOCTYPE html>
<html>
<body>

<div id="hasil"></div>

<script>
// Check browser support
if (typeof(Storage) !== "undefined") {
  // Store
  localStorage.setItem("contoh", "Rafi");
  // Retrieve
  document.getElementById("hasil").innerHTML = localStorage.getItem("contoh");
} else {
  document.getElementById("hasil").innerHTML = "Maaf, browser anda tidak mendukung";
}
</script>

</body>
</html>
<!-- Output : Rafi -->
```
```sh
Penjelasan : 
- Membuat pasangan nama/nilai localStorage dengan name="contoh1" dan value="Rafi"
- Ambil nilai "contoh1" dan masukkan ke dalam elemen dengan id="contoh"
```
- Kita bisa menghapus "contoh" pada localStorage dengan :
```js
// Menghapus berdasarkan 'key'
localStorage.removeItem("contoh");

// menghapus seluruh item pada local storage sekaligus
localStorage.clear();
```
- Pasangan nama/nilai selalu disimpan sebagai string.
- Objek sessionStorage sama dengan objek localStorage, kecuali objek tersebut menyimpan data hanya untuk satu sesi. Data dihapus ketika pengguna menutup tab browser tertentu.
- Contoh : 
```js
<!DOCTYPE html>
<html>
<body>

<div id="hasil"></div>

<script>
// Check browser support
if (typeof(Storage) !== "undefined") {
  // Store
  sessionStorage.setItem("contoh", "Rafi");
  // Retrieve
  document.getElementById("hasil").innerHTML = sessionStorage.getItem("contoh");
} else {
  document.getElementById("hasil").innerHTML = "Maaf, browser anda tidak mendukung";
}
</script>
</body>
</html>
<!-- Output : Rafi -->
```
```js
// Menghapus berdasarkan 'key'
sessionStorage.removeItem("contoh");

// menghapus seluruh item pada local storage sekaligus
sessionStorage.clear();
```
