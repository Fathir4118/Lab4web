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

![gambar]() 

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

![gambar]() 

**Buat Layout Sederhana**
Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css.

