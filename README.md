# lab4web
## Nama  : Zalfa Dewi Zahrani
## Nim   : 312210320
## Kelas : TI.22.A3
## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama ```Lab4Web```
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org
## Langkah-Langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file ```lab4_box.html``` seperti berikut.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>
</body>
```

## Membuat Box Element
Kemudian tambahkan kode untuk membuat ```box element``` dengan tag div seperti berikut.

```
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
</section>
```

## CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat ```float element```, seperti berikut.

```
<style>
    div {
    float:left;
    padding: 10px;
    }
    .div1 {
    background: red;
    }
    .div2 {
    background: yellow;
    }
    .div3 {
    background: green;
    }
</style>
</html>
```

## Mengatur Clearfix Element
-```Clearfix``` digunakan untuk mengatur element setelah ```float element```. ```Property``` clear digunakan untuk mengaturnya.

-Tambahkan ```element div``` lainnya seteleah div3 seperti berikut.

```
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
</section>
```

Kemudian atur ```property clear``` pada CSS, seperti berikut.

```
<style>
    div {
    float:left;
    padding: 10px;
    }
    .div1 {
    background: red;
    }
    .div2 {
    background: yellow;
    }
    .div3 {
    background: green;
    }
    .div4 {
background-color: blue;
clear: left;
float: none;
}
</style>
</html>
```

## Hasil Output

![Screenshot (257)](https://github.com/zalfadz05/lab4web/assets/115516617/118e64fa-1633-485a-af9f-cac8eeb1cbb3)

## Membuat Layout Sederhana
Kita akan membuat layout web sederhana seperti gambar berikut.



## Buat folder baru dengan nama ```lab4_layout``` , kemudian buatlah file baru didalamnya dengan nama ```home.html``` , dan file CSS dengan nama ```style.css```

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">

    </div>
</body>
```

## Kemudian tulis kode berikut.

```
<header>
    <h1>Layout Sederhana</h1>
</header>
<nav>
    <a href="home.html" class="active">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
</nav>
<section id="hero"></section>
<section id="wrapper">
    <section id="main"></section>
    <aside id="sidebar"></aside>
</section>
<footer>
    <p>&copy; 2023 - Universitas Pelita Bangsa</p>
</footer>
```

## Hasil Output

![Screenshot (258)](https://github.com/zalfadz05/lab4web/assets/115516617/320207bf-b157-4dd4-a2cc-ae5c1d9f9513)

## Kemudian tambahkan kode CSS untuk membuat layout nya.

```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
    padding: 20px;
}
header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

## Hasil Output

