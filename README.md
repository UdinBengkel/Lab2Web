# Lab2Web
html &amp; css

## Nama: Syafarudiansya
## NIM: 312410381
## Kelas: TI 24 A6

Penjelasan Praktikum

1. Mendeklarasikan CSS Internal

CSS internal adalah cara menulis aturan CSS langsung di dalam file HTML dengan menggunakan tag <style> di bagian <head>. Dengan cara ini, styling untuk elemen-elemen di halaman bisa diatur tanpa harus bikin file CSS terpisah.

```html
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
<img src="gambar/2.png" width="500"/>

2. Menambahkan Inline CSS

Inline CSS adalah cara memberi gaya langsung ke elemen HTML lewat atribut style di dalam tag elemen tersebut. Jadi aturan CSS hanya berlaku pada elemen yang ditulis, bukan ke elemen lain.

```html
<p style="text-align: center; color: #ccd8e4;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</>
```
<img src="gambar/3.png" width="500"/>

3. Membuat CSS Eksternal

CSS eksternal artinya aturan gaya (style) disimpan di file terpisah, misalnya style.css, lalu dipanggil ke dalam file HTML dengan `<link rel="stylesheet" href="style.css">` di bagian <head>. Jadi, HTML hanya berisi struktur konten (judul, paragraf, gambar, navigasi, dll), sementara file CSS khusus mengatur tampilannya (warna, ukuran, posisi, margin, padding, dsb).

```html
<head>
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```
Isi css eksternal:

```css
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
<img src="gambar/3.png" width="500"/>

4. Menambahkan CSS Selector

CSS Selector dipakai untuk memilih elemen HTML agar bisa diberi gaya. ID Selector `#` digunakan untuk elemen unik dalam halaman, sedangkan Class Selector `.` bisa dipakai berulang kali pada banyak elemen sehingga lebih fleksibel.

```css
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
<img src="gambar/5.png" width="500"/>
