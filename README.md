  # Lab2web
Nama : Mohammad Azmi Abdussyukur

NIM  : 312210109

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksipraktikum)|
|2|Praktikum|[Click Here](#praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaandantugas)|

## Instruksi Praktikum 
> 1. Persiapkan text editor misalnya VSCode.
> 2. Buat file baru dengan nama `lab2_css_dasar.html`
> 3. Buat struktur dasar dari dokumen HTML.
> 4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
> 5. Lakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/


## Praktikum 
### 1. Membuat dokumen HTML
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Dasar</title>
  </head>
  <body>
    <header>
      <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
      <a href="lab2_css_dasar.html">CSS Dasar</a>
      <a href="lab2_css_eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p>
        Kami sedang belajar HTML dan CSS dasar, pada mata kuliah
        <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran
        pertama yang kami dapat adalah membuat tampilan web sederhana dalam
        rangka mengenal tag-tag dasar HTML dan CSS.
      </p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
    </div>
  </body>
</html>
```
> - Maka hasilnya akan seperti berikut : 

<img width="960" alt="Cuplikan layar 2023-10-09 112417" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/07773b53-ac42-4427-83f6-5f0ccf38c7d0">


### 2. Mendeklerasikan CSS Internal
```
<head>
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>
```
> - Maka hasilnya akan seperti berikut :

<img width="960" alt="css in" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/024e485d-8437-4c08-8143-696da30e660a">

 
> - CSS internal adalah css yang filenya di letakan dalam html dengan pendeklarasian style.


### 3. Menambahkan Inline CSS
> - Menambahkan Inline CSS, kemudian tambahkan deklarasi inline CSS pada tag `<p>`
```
<p style="text-align: center; color: #ccd8e4;">
```
> - Maka hasilnya akan seperti berikut :

<img width="960" alt="4" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/ad57669a-3982-4efa-aaf6-32a1d06198e3">



### 4. Membuat CSS Eksternal
> - Membuat CSS Eksternal dengan membuat file baru dengan nama **style_eksternal.css** kemudian buat deklarasi css seperti berikut ini.
```
nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}
```
> - Kemudian tambahkan <link untuk merujuk File CSS yang telah dibuat pada bagian `<head>`
```
<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```

> - Maka hasilnya akan seperti berikut :

<img width="960" alt="Hasil dari css eksternal" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/bc68ec3c-a616-4655-9645-dbfa5999606d">


> - CSS ekternal adalah CSS yang file di tempatkan di luar file HTML dengan menambahkan link dalam HTML agar tertaut dengan file CSS

### 5. Menambahkan CSS Selector
> - Selanjutnya menambahkan CSS Selector menggunkan ID dan class Selector pada file **style_eksternal.css** dan menambahkan kode seperti berikut :
```
/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}
```
> - Maka hasilnya akan seperti berikut :

<img width="960" alt="hasill css 2" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/0fc00f7a-032d-4e32-9082-e3ded932c77b">


> - CSS Selector terdiri atas selector ID, Selector Class, Dan Selector elemen Selector ID pendeklarasiannya yaitu dengan (#), Sedangkan Class pendeklarasiannya yaitu dengan (.), Dan Selector elemen pendeklarasiannya dengan elemen HTML sebagai contoh (p) yang akan di beri gaya pada CSS.

### 6. MeLakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/

<img width="960" alt="check css 1" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/7b60ea76-5e1d-4ce5-a17c-3c61847065c2">


<img width="960" alt="validasi css" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/10526cee-77e7-45d8-95a9-450290d17f74">


## Pertanyaan dan Tugas 

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
> Jawaban :

<img width="960" alt="jawaban1html" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/20c64b18-9291-485d-bc85-60af595e4c82">


<img width="960" alt="jawaban1css" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/9a1542e8-ae15-4195-81cb-0763196edb20">


- Pada contoh ini, terdapat elemen `<h1> dengan class "title"` dan `elemen <p> dengan class "text"`. Class tersebut akan digunakan sebagai selector dalam CSS untuk mengubah properti dan nilai. Dalam file CSS (style.css), terdapat aturan CSS yang dideklarasikan untuk `class "title" dan "text"`. Aturan tersebut mengubah properti `"color"` pada elemen dengan class tersebut. Anda dapat mengubah nilai properti `"color"` pada file CSS sesuai keinginan Anda untuk melihat perubahan yang terjadi pada `judul (h1)` dan `paragraf (p)` dalam hal warna teks.


2. Apa perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}?` berikan penjelasannya!
> Jawaban :

- `h1 {...}` : Deklarasi ini akan merubah semua elemen "h1".

- `#intro h1 {...}` : Deklarasi ini lebih spesifik, maksud nya adalah pendeklarasian yang mengacu kepada pemberian atribut pada elemen "h1" dengan menambahkan id "intro".


3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
> Jawaban :

- Ketika kita mendeklarasikan secara bersamaan antara **INTERNAL EKSTERNAL** dan **INLINE** yang akan ditampilkan pada Browser adalah **INLINE**, karena **INLINE** memiliki prioritas dibanding **EKSTERNAL** atau pun **INTERNAL** seperti contoh yang saya buat, saya membuat dokumen baru HTML kemudian saya buat Elemen `{h1}`yang kemudian saya akan deklarasikan di CSS **INTERNAL EKSTERNAL** dan juga **INLINE** Dengan property `{color}` dengan warna yang berbeda,jika **INTERNAL** `{color: red}` sementara **EKSTERNAL** `{color:blue;}` dan **INLINE** `{color: green;}` yang terpanggil dibrowser adalah **INLINE** karena memiliki prioritas.


<img width="960" alt="jawaban3html" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/6e4818f7-09f6-4a2b-bd45-681cef7a74ef">

- Pict di atas adalah deklarasi **INLINE** dan **INTERNAL**, sementara pict di bawah adalah deklarasi **EKSTERNAL**.


<img width="960" alt="jawaban3css" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/fb222c0e-b1af-4314-982d-fa826cf5cc0c">

- Jadi yang terpanggil adalah **CSS INLINE** karena memiliki prioritas tinggi dibanding CSS deklarasi lainnya.


4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
> Jawaban :

```
( <p id="paragraf-1" class="text-paragraf"> )
```
- Yang terpanggil di browser adalah **ID** karena **ID** bersifat unik berbeda dengan **Class**. **Class** bisa digunakan banyak sementara **ID** hanya tertentu saja itu kenapa **ID** unik dan yang terpanggil di browser adalah **ID**.


<img width="960" alt="jawaban4html" src="https://github.com/MohAzmii04/Lab2web/assets/115864496/3ec549c4-7bbc-4367-9cfd-35dec8f6c496">

- Di atas saya menambahkan property `{color}` dan `{text-align}` untuk **ID {color: orchid}** dan **{text-align: center}** sementara Class yaitu **{color:palegreen}** dan **{text-align: left}**. Namun yang terpanggil di browser adalah **ID** yang property nya **{color: orchid}** dan juga **{text-align: center}**



## Finish, Terima Kasih 
