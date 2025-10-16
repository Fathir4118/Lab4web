# Lab4web


**Langkah-langkah Praktikum**

Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.

```html
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
</html>
```

**Membuat Box Element**
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.

```html
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div> 
</section>
```

**CSS Float Property**
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.

```html
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
```

**Hasil :**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005330.jpg) 

**Mengatur Clearfix Element**

Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya.

Tambahkan element div lainnya seteleah div3. Kemudian atur property clear pada CSS, seperti berikut.

```html
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div>
 <div class="div4">div 4</div>
 <div class="div5">div 5</div>
</section>
```

```html
.div4 {
 background: #ADD8E6;
 clear: right;
 float: none;
 }
 .div5 {
   background: #4863A0;
   clear: left;
   float: none;
 }
```

**Hasil :**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005345.jpg) 

**Buat Layout Sederhana**

Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css.

```html
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
</html>
```

```html
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
 <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

**hasil:**

![gambar]() 

Kemudian tambahkan kode CSS untuk membuat layoutnya.

```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&display=swap');
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

**Hasil :**

! [gambar]() 

**Membuat Navigasi**

Kemudian selanjutnya mengatur navigasi.

```css
nav {
 display: block;
 background-color: #1f5faa;
}
nav a {
 padding: 15px 30px;
 display: inline-block;
 color: #ffffff;
 font-size: 14px;
 text-decoration: none;
 font-weight: bold;
}
nav a.active,
nav a:hover {
 background-color: #2b83ea;
}
```

**Membuat Hero Panel**

Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.

```html
<section id="hero">
 <h1>Hello World!</h1>
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
 <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```

```css
#hero {
 background-color: #e4e4e5;
 padding: 50px 20px;
 margin-bottom: 20px;
}
#hero h1 {
 margin-bottom: 20px;
 font-size: 35px;
}
#hero p {
 margin-bottom: 20px;
 font-size: 18px;
 line-height: 25px;
}
```

**Hasil :**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005330.jpg) 

**Mengatur Layout Main dan Sidebar**

Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.

```css
#wrapper {
 margin: 0;
}
#main {
 float: left;
 width: 640px;
 padding: 20px;
}
/* sidebar area */
#sidebar {
 float: left;
 width: 260px;
 padding: 20px;
}
```

**Membuat Sidebar Widget**

Kemudian selanjutnya menambahkan element lain dalam sidebar.

```html
<aside id="sidebar">
 <div class="widget-box">
 <h3 class="title">Widget Header</h3>
 <ul>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 </ul>
 </div>
 <div class="widget-box">
 <h3 class="title">Widget Text</h3>
 <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
pharetra est nunc, nec pretium nunc pretium ac.</p>
 </div>
</aside>
```

Kemudian tambahkan CSS

```css
.widget-box {
 border:1px solid #eee;
 margin-bottom:20px;
}
.widget-box .title {
 padding:10px 16px;
 background-color:#428bca;
 color:#fff;
}
.widget-box ul {
 list-style-type:none;
}
.widget-box li {
 border-bottom:1px solid #eee;
}
.widget-box li a {
 padding:10px 16px;
 color:#333;
 display:block;
 text-decoration:none;
}
.widget-box li:hover a {
 background-color:#eee;
}
.widget-box p {
 padding:15px;
 line-height:25px;
}
```

**Hasil :**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005345.jpg) 

**Menambahkan Elemen lainnya pada Main Content**

```html
<section id="main">
 <div class="row">
 <div class="box">
 <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
 <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
 <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 </div>
</section>
```

Kemudian Tambahkan CSS

```css
/* box */
.box {
 display:block;
 float:left;
 width:33.333333%;
 box-sizing:border-box;
 -moz-box-sizing:border-box;
 -webkit-box-sizing:border-box;padding:0 10px;
 text-align:center;
}
.box h3 {
 margin: 15px 0;
}
.box p {
 line-height: 20px;
 font-size: 14px;
 margin-bottom: 15px;
}
box img {
 border: 0;
 vertical-align: middle;
}
.image-circle {
 border-radius: 50%;
}
.row {
 margin: 0 -10px;
 box-sizing: border-box;
 -moz-box-sizing: border-box;
 -webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
 content:'';
 display:table;
}
.row:after,
.entry:after {
 clear:both;
}
```

**Hasil :**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005403.jpg) 

**Menambahkan Content Artikel**

Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.

```html
<hr class="divider" />
<article class="entry">
 <h2>First featurette heading.</h2>
 <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
 <h2>First featurette heading.</h2>
 <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
</article>
```

Tambahkan CSS
```css
.divider {
 border:0;
 border-top:1px solid #eeeeee;
 margin:40px 0;
}
/* entry */
.entry {
 margin: 15px 0;
}
.entry h2 {
 margin-bottom: 20px;
}
.entry p {
 line-height: 25px;
}
.entry img {
 float: left;
 border-radius: 5px;
 margin-right: 15px;
}
.entry .right-img {
 float: right;
}
```

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005418.jpg) 

## **TUGAS!**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005523.jpg) 

# Hasil :

**CODE HTML**
```html
<!DOCTYPE html>
<html lang="en"
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Layout Sederhana</title>
 <link rel="stylesheet" href="stylee.css">
 </head>
<header>
 <h1>Layout Sederhana</h1>
</header>
<section id="hero">
 <h1>Hello World!</h1>
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
 <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
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
<section id="main">
 <div class="row">
 <div class="box">
 <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
 <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
 <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 </div>
<hr class="divider" />
<article class="entry">
 <h2>First featurette heading.</h2>
 <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
 <h2>First featurette heading.</h2>
 <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
</article>
</section>

<body>

<aside id="sidebar">
 <div class="widget-box">
 <h3 class="title">Widget Header</h3>
 <ul>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 </ul>
 </div>
 <div class="widget-box">
 <h3 class="title">Widget Text</h3>
 <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
pharetra est nunc, nec pretium nunc pretium ac.</p>
 </div>
</aside>
 
 <div id="container">
 </div>
 
<section id="form-section">
  <h2>Hubungi Saya</h2>
  <form>
    <label>Nama:</label><br>
    <input type="text" name="nama" required><br><br>
    <label>NIM:</label><br>
    <input type="text" name="nim" required><br><br>
    <label>Email:</label><br>
    <input type="email" name="email" required><br><br>
    <label>Nomor HP:</label><br>
    <input type="tel" name="nomor" required><br><br>
    <label>Message:</label><br>
    <textarea name="message" rows="4" required></textarea><br><br>
    <button type="submit">Kirim</button>
  </form>
</section>
<footer>
 <p>&copy; 2018 - Muhammad Fathir Nurcholis</p>
</footer>
</body>
</html>
```

**Code HTML Single Layout**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Single Layout</title>
  <link rel="stylesheet" href="stylee.css">
</head>
<body>
<header>
<nav>
 <a href="Lab4_layout.html">Home</a>
 <a href="artikel.html">Artikel</a>
 <a href="about.html" class=active>About</a>
 <a href="kontak.html">Kontak</a>
</nav>

  <h1>Single Layout</h1>
</header>

<section id="content">
  <h2>Deskripsi</h2>
  <h3>Hai..., Saya Muhammad Fathir Nurcholis</h3>
  <p>
    Halo! Ini adalah halaman deskripsi singkat tentang saya atau projek yang sedang saya kerjakan.
    Kamu bisa mengubah tulisan ini sesuai kebutuhan.
  </p>

  <h2>Portofolio</h2>
  <ul>
    <li><a href="#">Project 1</a></li>
    <li><a href="#">Project 2</a></li>
    <li><a href="#">Project 3</a></li>
    <li><a href="#">Project 4</a></li>
  </ul>
</section>
<footer>
  <p>&copy; 2018 - Muhammad Fathir Nurcholis</p>
</footer>
</body>
</html>
```

**Code style CSS**

```css
/* import google font */ 
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&display=swap');

/* ==== Form Section ==== */
#form-section {
  width: 80%;
  margin: 40px auto;
  padding: 20px;
  background: #f2f2f2;
  border-radius: 8px;
}

#form-section h2 {
  margin-bottom: 15px;
  color: #333;
}

#form-section form {
  display: flex;
  flex-direction: column;
}

#form-section label {
  font-weight: bold;
  margin-bottom: 5px;
}

#form-section input,
#form-section textarea {
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #bbb;
  border-radius: 5px;
}

#form-section button {
  width: 120px;
  padding: 10px;
  cursor: pointer;
  border: none;
  background: #0077cc;
  color: white;
  border-radius: 5px;
  font-size: 15px;
}

#form-section button:hover {
  background: #005fa3;
}

/* ==== Single Layout Page ==== */
#content {
  width: 80%;
  margin: 40px auto;
  padding: 20px;
  background: #f8f8f8;
  border-radius: 8px;
}

#content h2 {
  margin-bottom: 10px;
  color: #333;
}

#content ul {
  list-style-type: none;
  padding: 0;
}

#content ul li {
  margin: 8px 0;
}

#content ul li a {
  text-decoration: none;
  color: #0077cc;
}

#content ul li a:hover {
  text-decoration: underline;
}

.divider {
 border:0;
 border-top:1px solid #eeeeee;
 margin:40px 0;
}
/* entry */
.entry {
 margin: 15px 0;
}
.entry h2 {
 margin-bottom: 20px;
}
.entry p {
 line-height: 25px;
}
.entry img {
 float: left;
 border-radius: 5px;
 margin-right: 15px;
}
.entry .right-img {
 float: right;
}

/* box */
.box {
 display:block;
 float:left;
 width:33.333333%;
 box-sizing:border-box;
 -moz-box-sizing:border-box;
 -webkit-box-sizing:border-box;
 padding:0 10px;
 text-align:center;
}
.box h3 {
 margin: 15px 0;
}
.box p {
 line-height: 20px;
 font-size: 14px;
 margin-bottom: 15px;
}
box img {
 border: 0;
 vertical-align: middle;
}
.image-circle {
 border-radius: 50%;
}
.row {
 margin: 0 -10px;
 box-sizing: border-box;
 -moz-box-sizing: border-box;
 -webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
 content:'';
 display:table;
}
.row:after,
.entry:after {
 clear:both;
}

.widget-box {
 border:1px solid #eee;
 margin-bottom:20px;
}
.widget-box .title {
 padding:10px 16px;
 background-color:#428bca;
 color:#fff;
}
.widget-box ul {
 list-style-type:none;
}
.widget-box li {
 border-bottom:1px solid #eee;
}
.widget-box li a {
 padding:10px 16px;
 color:#333;
 display:block;
 text-decoration:none;
}
.widget-box li:hover a {
 background-color:#eee;
}
.widget-box p {
 padding:15px;
 line-height:25px;
}

#wrapper {
 margin: 0;
}
#main {
 float: left;
 width: 640px;
 padding: 20px;
}
/* sidebar area */
#sidebar {
 float: left;
 width: 260px;
 padding: 20px;
}
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

/* navigasi */ 
nav { 
    display: block; 
    background-color: #FFA500; 
} 
nav a { 
    padding: 15px 30px; 
    display: inline-block; 
    color: #ffffff; 
    font-size: 14px; 
    text-decoration: none; 
    font-weight: bold; 
} 
nav a.active, nav a:hover { 
    background-color: #000; 
} 

/* Hero Panel */ 
#hero { 
    background-color: #FFBF00; 
    padding: 50px 20px; 
    margin-bottom: 20px; 
} 
#hero h1 { 
    margin-bottom: 20px; 
    font-size: 35px; 
} 
#hero p { 
    margin-bottom: 20px; 
    font-size: 18px; 
    line-height: 25px; 
}

/* main content dan sidebar */ 
#wrapper { margin: 0; } 
#main { float: left; width: 640px; padding: 20px; } 
#sidebar { float: left; width: 260px; padding: 20px; }

/* widget */ 
.widget-box { border:1px solid #FFBF00; margin-bottom:20px; } 
.widget-box .title { padding:10px 16px; background-color:#FFFF00; color:#000; } 
.widget-box ul { list-style-type:none; } 
.widget-box li { border-bottom:1px solid #FFBF00; } 
.widget-box li a { padding:10px 16px; color:#333; display:block; text-decoration:none; } 
.widget-box li:hover a { background-color:#FFBF00; } 
.widget-box p { padding:15px; line-height:25px; }

/* footer */ 
footer { 
    clear:both; 
    background-color:#1d1d1d; 
    padding:20px; 
    color:#eee; 
}
```

# **Tampilan WEB**

**Home**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005442.jpg) 

**About**

![gambar](https://github.com/Fathir4118/Lab4web/blob/main/Gambar/IMG_20251017_005500.jpg) 
