# Praktikum 4 - Pemograman Web
```
Riska Puspa Anggraeni Putri
TI.19.A2
311910440
```
## Langkah 1
### Membuat dokumen HTML dengan nama file lab4_box.html. Setelah itu buat struktur dasar HTML
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
</html>
```
![1](https://user-images.githubusercontent.com/56241285/115221396-d1c9cf00-a133-11eb-887e-a8f80de2876c.png)
## Langkah 2
### Membuat Box Element
```
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div> 
</section>
```
![2](https://user-images.githubusercontent.com/56241285/115221575-06d62180-a134-11eb-8f4e-fe9d262570e9.png)
## Langkah 3
### CSS Float Property
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
```
![3](https://user-images.githubusercontent.com/56241285/115221913-5ae10600-a134-11eb-90dc-86b480898499.png)
## Langkah 4
### Mengatur Clearfix Element
#### Tambahkan element div lainnya seteleah div3
```
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div> 
 <div class="div4">Div 4</div> 
</section>
```
![4](https://user-images.githubusercontent.com/56241285/115223257-cbd4ed80-a135-11eb-9526-50412ee88972.png)
#### Kemudian atur property clear pada CSS
```
.div4 {
background-color: blue;
clear: left;
float: none;
}
```
![5](https://user-images.githubusercontent.com/56241285/115223546-1bb3b480-a136-11eb-9d71-54fc8cbd7cf8.png)
## Langkah 5
### Membuat Layout Sederhana dengan folder baru dengan nama lab4_layout , kemudian Membuat dokumen HTML dengan nama file home.html, dan file css dengan nama style.css. Setelah itu buat struktur dasar HTML ke file home.html
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
</html>
```
![7](https://user-images.githubusercontent.com/56241285/115227352-8e269380-a13a-11eb-922b-32a2ffbbb2d9.png)
![8](https://user-images.githubusercontent.com/56241285/115227436-a9919e80-a13a-11eb-82c5-501cc07c9ca5.png)
#### Kemudian tulis kode
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
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
           </footer>
```
![6](https://user-images.githubusercontent.com/56241285/115226784-d4c7be00-a139-11eb-974e-84c7169ae876.png)
#### Kemudian tambahkan kode CSS untuk membuat layoutnya
