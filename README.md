[![banner.png](https://i.postimg.cc/0NcgTNhZ/banner.png)](https://postimg.cc/PLpFZdX8)
# Proyecto n°3: Landing de Negocio.

------------

<p>
 
En este proyecto se dará a conocer la construcción de una página web dirigida a un `Landign de Negocio` el cual se realizará con el lenguaje de programación `HTML` y `CSS` donde se utilizará el editor `Studio Visual Code` para codificar el sitio web. A continuación, se darán a conocer los requisitos del proyecto y el paso a paso de su construcción.

</p>

------------

## Requisitos del Proyecto.

------------

-  Desarrollar prototipado simple.
-  Aplicar en todo el sitio HTML5
-  Aplicar estilos CSS.
-  Sección Header.
-  Sección Main
-  Sección Products.
-  Sección Footer.
-  Opcional. Responsive Web Design (Vista en móviles con uso de media queries).

------------

## Realización página web paso a paso.

------------

<p>
 
En la construcción de diseño del `Landing de Negocio` se realizó primero en un archivo `index.html` y en otro archivo llamado `style.css` se confeccionaron los estilos de la página web, además se creó una carpeta el cual contiene todas las imágenes incluidas en el proyecto. 

</p>

1. Primero creamos el `Header` el cual contiene los primeros elementos de la página web que son el logo, titulo y barra de navegación.
   

```html
 <!-- Header -->
    <header>
        <div class="logo">
            <img src="fotos.jpg\logo2.png" alt="Logo Agencia de Viajes">
        </div>
        <nav>
            <div class="titulo_mochilero">
                Mochileros Por El Mundo!
            </div>
            <ul>
                <li><a href="#">Inicio</a></li>
                <li><a href="#">Destinos</a></li>
                <li><a href="#">Viajes</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </nav>
    </header>
```

<p>Luego se muestran los estilos brindados en el `Header`.</p>


```css
/* Estilos generales */
body {
    font-family: "DM Serif Text", serif;
    margin: 0;
    padding: 0;
}

a {
    
    text-decoration: none;
    color: black;
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #ffff;
    color: black;
}

.logo img {
    max-height: 140px;
    border-radius: 50%;
}

.titulo_mochilero {
    font-family: "Lilita One", sans-serif;
    font-size:30px;
    font-weight: bold;
    letter-spacing: 10px;
    color: black;
    position: absolute;
    left: 50%;
    transform: translateX(-75%);
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    color: black;
    font-weight: bold;
    cursor:pointer;
    
}
```

2. Se crea el contenido del `Main` que es el bloque de código el cual contendrá la parte principal de la página web.
   

```html
 <!-- Main -->
    <main style="background-image: url('fotos.jpg/comboya2.JPG'); background-size: cover; background-position: center;">
        <section class="presentation">
            <h1 class="titulo_presentation">Bienvenido a nuestra agencia de Viajes</h1>
            <p class="titulo_presentation">Explora el mundo con nosotros aprovecha de nuestros servicios personalizados y disfruta de una experiencia única.</p>
            <p class="titulo_presentation">Embárcate en un viaje inolvidable. Nuestros servicios se enfocan en programar y personalizar tu viaje junto a nuestros grandes guías turísticos y nuestro equipo en conjunto haremos que vivas una experiencia que jamás olvidaras.</p>
            <form class="titulo_presentation">
                <label for="email">Introduce tu correo para más información:</label>
                <input type="email" id="email" name="email" placeholder="tuemail@ejemplo.com">
                <button type="submit">Suscribirse</button>
            </form>
        </section>
    </main>

```

<p>
 
Luego tenemos el diseño de estilos brindado en el `Main`.

</p>

```css
/* Main */
main {
    padding: 50px;
    background-color: #f9f9f9;
    text-align: center;
}

.presentation {
    max-width: none;
    background-color: black;
    opacity: 80%;
    margin: auto;
    padding: inherit;
}

.titulo_presentation{
    color: white;
    opacity: 100%;
}

.presentation form {
    margin-top: 20px;
}

.presentation input[type="email"] {
    padding: 10px;
    margin-right: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.presentation button {
    padding: 10px 20px;
    border: none;
    background-color: #1e5b9b;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

```

<p>
 
3. Seguimos con la construcción de la página web y tenemos la sección `Productos`.
   
</p>


```html
 <!-- Productos -->
    <section class="products">
        <h2>Nuestros Viajes Programados Por El Sudeste Asíatico</h2>
        <div class="product-list">
            <article class="product">
                <img src="fotos.jpg/camboya4.JPG" alt="Producto 1">
                <h3>Tour por Camboya</h3>
                <p>Explora las maravillas de Camboya.</p>
            </article>
            <article class="product">
                <img src="fotos.jpg/tailandia6.JPG" alt="Producto 2">
                <h3>Tour por Tailandia</h3>
                <p>Descubre los encantos de Tailandia.</p>
            </article>
            <article class="product">
                <img src="fotos.jpg\india4.JPG" alt="Producto 3">
                <h3>Tour por India</h3>
                <p>Descubre los hermosos templos de la India.</p>
            </article>
        </div>
    </section>

    <div class="horizontal-scroll">
        <img src="fotos.jpg/vietnam6.JPG" alt="Imagen 1">
        <img src="fotos.jpg/vietnam5.JPG" alt="Imagen 2">
        <img src="fotos.jpg/camboya3.JPG" alt="Imagen 3">
        <img src="fotos.jpg/turista1.JPG" alt="Imagen 4">
        <img src="fotos.jpg/tailandia4.JPG" alt="Imagen 5">
        <img src="fotos.jpg/tailandia2.JPG" alt="Imagen 1">
        <img src="fotos.jpg/tailandia1.JPG" alt="Imagen 2">
        <img src="fotos.jpg/india3.JPG" alt="Imagen 3">
        <img src="fotos.jpg/india1.JPG" alt="Imagen 4">
        <img src="fotos.jpg/india2.JPG" alt="Imagen 5">
        <img src="fotos.jpg/comboya1.JPG" alt="Imagen 1">
        <img src="fotos.jpg/camboya5.JPG" alt="Imagen 2">
        <img src="fotos.jpg/vietnam2.JPG" alt="Imagen 3">
        <img src="fotos.jpg/vietnam3.JPG" alt="Imagen 4">
        <img src="fotos.jpg/DSC00802.JPG" alt="Imagen 5">

    </div>
```

<p>
 
Luego tenemos el diseño de estilos brindado en `Productos`.

</p>

```css
/* Products */
.products {
    padding: 50px;
    background-color: white;
    text-align: center;
}

.product-list {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.product {
    max-width: 300px;
    border: 1px solid #ccc;
    border-radius: 10px;
    overflow: hidden;
    transition: 400ms all; 
    cursor: pointer
}
.product:hover{
    transform: scale(1.1);
}
 
.product img {
    width: 100%;
    height: auto;
    transition: 400ms all;
}

.product h3 {
    padding: 10px;
}

.product p {
    padding: 0 10px 10px 10px;
}

.product img:hover {
    transform: scale(1.1);
}

.horizontal-scroll {
    width: 100%;
    overflow-x: auto;
    display: flex;
    align-items: center;
    white-space: nowrap;
    height: 150px;  /* Altura fija del contenedor */
}

.horizontal-scroll img {
    max-height: 100%;  /* Las imágenes no excederán la altura del contenedor */
    max-width: 100%;  /* Previene que las imágenes sean más anchas que el contenedor */
    width: auto;      /* Mantiene la relación de aspecto de las imágenes */
    height: auto;     /* Mantiene la relación de aspecto de las imágenes */
    margin-right: 10px; /* Espacio entre imágenes */
    transition: 400ms all;
    cursor: pointer;
}

.horizontal-scroll img:hover{
    transform:scale(1.1)
}

```

<p>
 
4. Y por último tenemos la sección del `Footer` que es la última parte del diseño web.
   
</p>


```html
  <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-social">
                <h1 class="final_footer">Síguenos</h1>
                <ul>
                    <li><a href="#"><img src="fotos.jpg/facebook.png" alt="Facebook"></a></li>
                    <li><a href="#"><img src="fotos.jpg/whatsapp (1).png" alt="Whatsapp"></a></li>
                    <li><a href="#"><img src="fotos.jpg/instagram.png" alt="Instagram"></a></li>
                    <li><a href="#"><img src="fotos.jpg/youtube.png" alt="Youtube"></a></li>
                </ul>
            </div>
        </div>
        <p>&copy; 2024 Agencia de Viajes. Todos los derechos reservados.</p>
    </footer>
</body>
</html>

```

<p>
 
Y también tenemos la última parte de los estilos brindados en el `Footer`.

</p>

```css
/* Footer */
footer {
    padding: 20px;
    background-color: #01080f;
    color: white;
    text-align: center;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.footer-social {
    margin: 30px 0;
}

.footer-social ul {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
    transform: translateX(160%);
}

.footer-social ul li img {
    max-height: 45px;
    transition: 400ms all;
    cursor: pointer;
}
.footer-social ul li img:hover {
    transform:scale(1.1)
}
.final_footer {
    transform: translateX(170%);
}
```

<p>
 
La solución final en conjunto de `HTML` sería así: 

</p>

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agencia de viajes</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lilita+One&display=swap" rel="stylesheet">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lilita+One&family=Permanent+Marker&display=swap" rel="stylesheet">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=DM+Serif+Text:ital@0;1&family=Lilita+One&family=Permanent+Marker&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="logo">
            <img src="fotos.jpg\logo2.png" alt="Logo Agencia de Viajes">
        </div>
        <nav>
            <div class="titulo_mochilero">
                Mochileros Por El Mundo!
            </div>
            <ul>
                <li><a href="#">Inicio</a></li>
                <li><a href="#">Destinos</a></li>
                <li><a href="#">Viajes</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main -->
    <main style="background-image: url('fotos.jpg/comboya2.JPG'); background-size: cover; background-position: center;">
        <section class="presentation">
            <h1 class="titulo_presentation">Bienvenido a nuestra agencia de Viajes</h1>
            <p class="titulo_presentation">Explora el mundo con nosotros aprovecha de nuestros servicios personalizados y disfruta de una experiencia única.</p>
            <p class="titulo_presentation">Embárcate en un viaje inolvidable. Nuestros servicios se enfocan en programar y personalizar tu viaje junto a nuestros grandes guías turísticos y nuestro equipo en conjunto haremos que vivas una experiencia que jamás olvidaras.</p>
            <form class="titulo_presentation">
                <label for="email">Introduce tu correo para más información:</label>
                <input type="email" id="email" name="email" placeholder="tuemail@ejemplo.com">
                <button type="submit">Suscribirse</button>
            </form>
        </section>
    </main>

    <!-- Productos -->
    <section class="products">
        <h2>Nuestros Viajes Programados Por El Sudeste Asíatico</h2>
        <div class="product-list">
            <article class="product">
                <img src="fotos.jpg/camboya4.JPG" alt="Producto 1">
                <h3>Tour por Camboya</h3>
                <p>Explora las maravillas de Camboya.</p>
            </article>
            <article class="product">
                <img src="fotos.jpg/tailandia6.JPG" alt="Producto 2">
                <h3>Tour por Tailandia</h3>
                <p>Descubre los encantos de Tailandia.</p>
            </article>
            <article class="product">
                <img src="fotos.jpg\india4.JPG" alt="Producto 3">
                <h3>Tour por India</h3>
                <p>Descubre los hermosos templos de la India.</p>
            </article>
        </div>
    </section>

    <div class="horizontal-scroll">
        <img src="fotos.jpg/vietnam6.JPG" alt="Imagen 1">
        <img src="fotos.jpg/vietnam5.JPG" alt="Imagen 2">
        <img src="fotos.jpg/camboya3.JPG" alt="Imagen 3">
        <img src="fotos.jpg/turista1.JPG" alt="Imagen 4">
        <img src="fotos.jpg/tailandia4.JPG" alt="Imagen 5">
        <img src="fotos.jpg/tailandia2.JPG" alt="Imagen 1">
        <img src="fotos.jpg/tailandia1.JPG" alt="Imagen 2">
        <img src="fotos.jpg/india3.JPG" alt="Imagen 3">
        <img src="fotos.jpg/india1.JPG" alt="Imagen 4">
        <img src="fotos.jpg/india2.JPG" alt="Imagen 5">
        <img src="fotos.jpg/comboya1.JPG" alt="Imagen 1">
        <img src="fotos.jpg/camboya5.JPG" alt="Imagen 2">
        <img src="fotos.jpg/vietnam2.JPG" alt="Imagen 3">
        <img src="fotos.jpg/vietnam3.JPG" alt="Imagen 4">
        <img src="fotos.jpg/DSC00802.JPG" alt="Imagen 5">

    </div>
    
    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-social">
                <h1 class="final_footer">Síguenos</h1>
                <ul>
                    <li><a href="#"><img src="fotos.jpg/facebook.png" alt="Facebook"></a></li>
                    <li><a href="#"><img src="fotos.jpg/whatsapp (1).png" alt="Whatsapp"></a></li>
                    <li><a href="#"><img src="fotos.jpg/instagram.png" alt="Instagram"></a></li>
                    <li><a href="#"><img src="fotos.jpg/youtube.png" alt="Youtube"></a></li>
                </ul>
            </div>
        </div>
        <p>&copy; 2024 Agencia de Viajes. Todos los derechos reservados.</p>
    </footer>
</body>
</html>

```

<p>
 
La solución final del diseño de estilos en `CSS` sería así:

</p>


```css
/* Estilos generales */
body {
    font-family: "DM Serif Text", serif;
    margin: 0;
    padding: 0;
}

a {
    
    text-decoration: none;
    color: black;
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #ffff;
    color: black;
}

.logo img {
    max-height: 140px;
    border-radius: 50%;
}

.titulo_mochilero {
    font-family: "Lilita One", sans-serif;
    font-size:30px;
    font-weight: bold;
    letter-spacing: 10px;
    color: black;
    position: absolute;
    left: 50%;
    transform: translateX(-75%);
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    color: black;
    font-weight: bold;
    cursor:pointer;
    
}

/* Main */
main {
    padding: 50px;
    background-color: #f9f9f9;
    text-align: center;
}

.presentation {
    max-width: none;
    background-color: black;
    opacity: 80%;
    margin: auto;
    padding: inherit;
}

.titulo_presentation{
    color: white;
    opacity: 100%;
}

.presentation form {
    margin-top: 20px;
}

.presentation input[type="email"] {
    padding: 10px;
    margin-right: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.presentation button {
    padding: 10px 20px;
    border: none;
    background-color: #1e5b9b;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

/* Products */
.products {
    padding: 50px;
    background-color: white;
    text-align: center;
}

.product-list {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.product {
    max-width: 300px;
    border: 1px solid #ccc;
    border-radius: 10px;
    overflow: hidden;
    transition: 400ms all; 
    cursor: pointer
}
.product:hover{
    transform: scale(1.1);
}
 
.product img {
    width: 100%;
    height: auto;
    transition: 400ms all;
}

.product h3 {
    padding: 10px;
}

.product p {
    padding: 0 10px 10px 10px;
}

.product img:hover {
    transform: scale(1.1);
}

.horizontal-scroll {
    width: 100%;
    overflow-x: auto;
    display: flex;
    align-items: center;
    white-space: nowrap;
    height: 150px;  /* Altura fija del contenedor */
}

.horizontal-scroll img {
    max-height: 100%;  /* Las imágenes no excederán la altura del contenedor */
    max-width: 100%;  /* Previene que las imágenes sean más anchas que el contenedor */
    width: auto;      /* Mantiene la relación de aspecto de las imágenes */
    height: auto;     /* Mantiene la relación de aspecto de las imágenes */
    margin-right: 10px; /* Espacio entre imágenes */
    transition: 400ms all;
    cursor: pointer;
}

.horizontal-scroll img:hover{
    transform:scale(1.1)
}

/* Footer */
footer {
    padding: 20px;
    background-color: #01080f;
    color: white;
    text-align: center;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.footer-social {
    margin: 30px 0;
}

.footer-social ul {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
    transform: translateX(160%);
}

.footer-social ul li img {
    max-height: 45px;
    transition: 400ms all;
    cursor: pointer;
}
.footer-social ul li img:hover {
    transform:scale(1.1)
}
.final_footer {
    transform: translateX(170%);
}
```
<p> A continuación se dara a conocer el prototipado de la página web antes de comenzar el desarrollo del proyecto: </p>

[![prototipo-dise-o.png](https://i.postimg.cc/d1JqPXWm/prototipo-dise-o.png)](https://postimg.cc/mc6x7dWt)

<p> La página Landing de Negocio finalizada se vería así: </p>

1. Sección Header:

[![dise-o-pagina-1.png](https://i.postimg.cc/Hkn1dc7r/dise-o-pagina-1.png)](https://postimg.cc/RNkDT0dm)

2. Sección Main:

[![dise-o-3.png](https://i.postimg.cc/B6Kqs8kT/dise-o-3.png)](https://postimg.cc/47XCQ3Jy)



