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
### Membuat Layout Sederhana 
#### buat folder baru dengan nama lab4_layout , kemudian Membuat dokumen HTML dengan nama file home.html, dan file css dengan nama style.css. Setelah itu buat struktur dasar HTML ke file home.html
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
![9](https://user-images.githubusercontent.com/56241285/115231871-486cc980-a140-11eb-9813-76c0a9c3a52d.png)
#### Membuat Navigasi
``` 
/* navigasi */
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
![10](https://user-images.githubusercontent.com/56241285/115232681-36d7f180-a141-11eb-8bc7-5c5a930b1155.png)
#### Membuat Hero Panel
##### Tambahkan kode HTML
```
<section id="hero">
 <h1>Hello World!</h1>
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
 <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
![11](https://user-images.githubusercontent.com/56241285/115234119-e19cdf80-a142-11eb-9d4e-1e7b63796cc2.png)
##### Tambahkan Kode CSS
``` 
/* Hero Panel */
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
![12](https://user-images.githubusercontent.com/56241285/115234912-c5e60900-a143-11eb-8809-c4cc08dce5b3.png)
#### Mengatur Layout Main dan Sidebar
```
/* main content */
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
![13](https://user-images.githubusercontent.com/56241285/115236003-072ae880-a145-11eb-81e6-de329d4edc9f.png)
#### Membuat Sidebar Widget
##### tambahkan di HTML
```
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
![14](https://user-images.githubusercontent.com/56241285/115236614-c1baeb00-a145-11eb-98f2-99a5198e46a2.png)
##### Tambahkan di CSS
```
* widget */
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
![15](https://user-images.githubusercontent.com/56241285/115237134-63dad300-a146-11eb-8575-a47b9cdfeef5.png)
#### Mengatur Footer
```
/* footer */
footer {
 clear:both;
 background-color:#1d1d1d;
 padding:20px;
 color:#eee;
}
```
![16](https://user-images.githubusercontent.com/56241285/115237648-ff6c4380-a146-11eb-8465-2413dc1f4c14.png)
#### Menambahkan Elemen lainnya pada Main Content
##### Tambahkan di HTML
```
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
![17](https://user-images.githubusercontent.com/56241285/115238270-b36dce80-a147-11eb-80a6-fa330de7b485.png)
##### Tambahkan di CSS
```
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
```
![18](https://user-images.githubusercontent.com/56241285/115239041-8bcb3600-a148-11eb-87ad-457d1da20c88.png)
#### Menambahkan Content Artikel
##### Tambahkan di HTML
```
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
![19](https://user-images.githubusercontent.com/56241285/115239555-13b14000-a149-11eb-9427-228e1da392ff.png)
##### Tambahkan di CSS
```
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
![20](https://user-images.githubusercontent.com/56241285/115240027-8c180100-a149-11eb-9c3c-c3df409c989e.png)
![21](https://user-images.githubusercontent.com/56241285/115240012-87ebe380-a149-11eb-8260-cc4714c79c97.png)
## Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
- buat single layout yang berisi deskripsi, portofolio, dll.
2. Tambahkan Layout untuk menu Contact
- yang berisi form isian: Nama, Email, Message, dll.
## Jawab 
### Tambahkan Layout untuk menu About
#### Membuat dokumen html dengan nama about.html. Setelah itu buat struktur dasar HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>About Me</h1>
        </header>
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="About.html">About</a>
            <a href="Kontak.html">Kontak</a>
        </nav>
        <section id="introduce">
            <div class="row">
                <img src="Riska.jpg" title="Riskapap" alt="Riskapap" class="image-circle" width="230"style="float: left; border: 2px solid black;">
                <h1>Hello!</h1>
                <p>Nama saya Riska Puspa Anggraeni Putri. Saya adalah seorang mahasiswa dari <b>Universitas Pelita Bangsa</b> yang saat ini sedang
                    mempelajari materi Layout CSS dalam mata kuliah <i>Pemrograman Web</i>.</p>
            </div>
        </section>
    </div>
</body>
</html>
```
![22](https://user-images.githubusercontent.com/56241285/115243196-dcdd2900-a14c-11eb-8c6b-0ee4192b0962.png)
#### Tambahkan di CSS
```
/* Introduce Panel */
 #introduce{
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#introduce h1 {
    margin-bottom: 10px;
    font-size: 35px;
    position: relative;
    left: 15px;
}
#introduce p {
    margin-bottom: 20px;
    font-size: 18px;
    padding: 30px;
    line-height: 25px;
    position: relative;
    left: 15px;
}
```
![23](https://user-images.githubusercontent.com/56241285/115246462-1c594480-a150-11eb-998a-15dba8120a87.png)
#### Hasil 
![24](https://user-images.githubusercontent.com/56241285/115248545-f92f9480-a151-11eb-8a55-6dc8daa67f03.png)
### Menambahkan Layout pada menu Contact
#### Membuat dokumen html dengan nama kontak.html. Setelah itu buat struktur dasar HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Contact Me</h1>
        </header>
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <section id="kontak">
            <div class="login">
                <input type="text" placeholder="Your Name" class="input">
                <input type="text" placeholder="Your Email Address" class="input">
            </div>

            <div class="subject">
                <input type="text" placeholder="Subject" class="input">
            </div>

            <div class="msg">
                <textarea class="area" cols="35" rows="10" placeholder="Your Message" class="input"></textarea>
            </div>

            <button type="submit"> Send </button>

        </section>
    </div>
</body>
</html>
```
![25](https://user-images.githubusercontent.com/56241285/115245600-4c541800-a14f-11eb-8eda-adf851fe7597.png)
#### Tambahkan di CSS
```
/* Contact Panel */
#kontak{
    background-color: #e4e4e5;
    padding: 20px 20px;
    margin-bottom: 20px;
}
.input,
.msg, .area{
    width: 100%;
    padding: 10px;
    border: 2px solid white;
    box-sizing: border-box;
    font-size: 15px;
    margin-bottom: 20px;
}
button{
    font-size: 14px;
    background-color: #3f3f3f;
    color: white;
    border-radius: 5px;
    padding: 10px 20px;
    margin-top: 8x;
}
button :hover{
    opacity: 0,9;
}
```
![26](https://user-images.githubusercontent.com/56241285/115247211-ccc74880-a150-11eb-928d-41c37a63a300.png)
#### Hasil
![27](https://user-images.githubusercontent.com/56241285/115248634-106e8200-a152-11eb-8488-d77430e582a6.png)
