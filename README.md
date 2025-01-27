# web
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muebles y Más JM</title>
    <link rel="stylesheet" href="styles.css">
    <!-- Inserción de la fuente Teko de Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Teko:wght@400;600&display=swap" rel="stylesheet">
    <style>

html, body {
    overflow-x: hidden; /* Evita el desplazamiento horizontal */
}

body {
    font-family: 'Teko', Arial, sans-serif; /* Aplicamos la fuente Teko a todo el contenido */
    margin: 0;
    padding: 0;
    background-color: #e9e9e9;
}

header {
    background-color: #333;
    padding: 1px 0; /* Reduce el padding */
}

nav {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    background-color: #4e280c;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    width: 100%; /* Asegura que la barra de navegación ocupe todo el ancho */
}

nav a {
    color: #fffbfb;
    padding: 10px 15px;
    text-decoration: none;
    transition: background-color 0.3s;
}

nav a:hover {
    background-color: #f0f0f0;
}

.logo {
    max-width: 80px;
    height: auto; /* Ajustar la altura automática para mantener la proporción */
}

.search-bar {
    display: flex;
    justify-content: center;
    margin: 20px 0;
}

.search-bar input {
    width: 300px;
    padding: 10px;
    border: 2px solid #ccc;
    border-radius: 25px; /* Bordes redondeados */
    outline: none;
    transition: all 0.3s;
}

.search-bar input:focus {
    border-color: #6d564a;
}

.container {
    padding: 20px;
}

.section {
    margin: 20px 0;
}

.section h2 {
    background-color: #4e280c;
    color: white;
    padding: 10px;
    text-align: center;
}

.product-list, .featured-products {
    display: flex;
    justify-content: space-around; /* Ajusta la justificación para mantener los productos juntos */
    gap: 20px; /* Añade espacio entre los productos */
}

.product, .featured-product {
    background-color: white;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 20px; /* Aumenta el padding del contenedor */
    width: calc(33.33% - 20px); /* Ajusta el ancho del contenedor del producto */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    overflow: hidden; /* Evita que el contenido se salga del contenedor */
}

.product img, .featured-product img {
    max-width: 100%; /* Ajusta el tamaño máximo de la imagen al 100% del contenedor */
    height: auto; /* Mantiene la proporción de la imagen */
    max-height: 150px; /* Ajusta la altura máxima de la imagen */
    margin-bottom: 10px; /* Añade espacio debajo de la imagen */
}

.product p, .featured-product p {
    margin: 5px 0; /* Espacio entre párrafos */
}

.product-price {
    color: red; /* Color del precio final */
    font-weight: bold;
}

.product-normal-price {
    text-decoration: line-through; /* Texto tachado para el precio normal */
}

footer {
    background-color: #333;
    color: white;
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: flex-start;
}

.footer-section {
    flex: 1;
    margin: 10px;
    min-width: 200px;
}

.footer-section h3 {
    color: #ffffff;
    margin-bottom: 10px;
    border-bottom: 2px solid #ddd; /* Línea decorativa */
    padding-bottom: 5px;
    text-align: center; /* Alineación centrada */
}

.footer-section ul {
    list-style: none;
    padding: 0;
}

.footer-section ul li {
    margin-bottom: 5px;
}

.footer-section ul li a {
    color: #ffffff;
    text-decoration: none;
    transition: color 0.3s;
}

.footer-section ul li a:hover {
    color: #dddddd;
}

.footer-social {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    bottom: 0;
    width: 100%;
    background-color: #333; /* Opcional: añade color de fondo */
    padding: 10px 0; /* Añade un poco de espacio alrededor del logo */
}

.footer-social a {
    margin: 0 10px;
}

.footer-social img {
    width: 30px;
}

.featured-product img {
    max-width: 100%; /* Ajusta el tamaño según sea necesario */
    height: auto;
    max-height: 150px; /* Ajusta la altura máxima de la imagen */
}

.logo img {
    max-width: 80px; /* Ajusta el tamaño máximo según sea necesario */
    height: auto; /* Mantiene la proporción de la imagen */
}

.hero-section {
    background-image: url("mu.png");
    background-size: cover;
    height: 400px; /* Ajusta la altura según necesites */
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 2em;
}

.hero-text-box {
    background-color: rgba(0, 0, 0, 0.5); /* Recuadro negro borroso */
    padding: 20px;
    border-radius: 5px;
    text-align: center;
}

.hero-text-box h1 {
    color: #ffffff; /* Color del texto */
    font-family: 'Teko', sans-serif;
    font-size: 36px; /* Tamaño de la letra */
}

.product img {
    max-width: 100%; /* Ajusta el tamaño máximo de la imagen al 100% del contenedor */
    height: auto; /* Mantiene la proporción de la imagen */
    max-height: 150px; /* Ajusta la altura máxima de la imagen */
    margin-bottom: 10px; /* Añade espacio debajo de la imagen */
}

.product {
    background-color: white;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 20px; /* Aumenta el padding del contenedor */
    width: calc(33.33% - 20px); /* Ajusta el ancho del contenedor del producto */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    overflow: hidden; /* Evita que el contenido se salga del contenedor */
}
    </style>
</head>
<body>
    <nav>
        <div class="logo">
            <img src="image.png" alt="Logo Muebles y Más JM">
        </div>
        <div>
            <a href="#inicio">Inicio</a>
            <a href="#productos">Productos</a>
            <a href="#contacto">Contacto</a>
        </div>
        <div class="search-bar">
            <input type="text" placeholder="Busca aquí por toda la tienda...">
        </div>
    </nav>
    <div class="hero-section">
        <div class="hero-text-box">
            <h1>Bienvenidos a Muebles y Más JM</h1>
            <p>Los mejores muebles para tu hogar.</p>
        </div>
    </div>
    <div class="container">
        <div class="section">
            <h2>Productos Destacados</h2>
            <div class="featured-products">
                <div class="featured-product">
                    <img src="produmas.png" alt="Escritorio Rosetta Blanco">
                    <h3>Soporte para Espada u Objeto</h3>
                    <p class="product-normal-price">Normal: $1,800.00</p>
                    <p>Precio Especial: $1,699.00</p>
                    <p class="product-price">Precio al Pagar: $850.00</p>
                </div>
                <div class="featured-product">
                    <img src="produ2.png" alt="Escritorio Brooklyn Café">
                    <h3>Mueble para Television Personalizable</h3>
                    <p class="product-normal-price">Normal: $5,400.00</p>
                    <p>Precio Especial: $4,149.00</p>
                    <p class="product-price">Precio al Pagar: $3,500.00</p>
                </div>
                <div class="featured-product">
                    <img src="3.png" alt="Escritorio Gamer Sparx Negro">
                    <h3>Soporte para pantalla de 32" a 75" simple</h3>
                    <p class="product-normal-price">Normal: $1,700.00</p>
                    <p>Precio Especial: $1,116.47</p>
                    <p class="product-price">Precio al Pagar: $1,200.00-$600.00</p>
                </div>
            </div>
        </div>
        <div class="section">
            <h2>OTROS PRODUCTOS</h2>
            <div class="product-list">
                    <div class="product">
                        <img src="4.png" alt="Producto A">
                        <h3>Closet Personalizable</h3>
                        <p class="product-normal-price">Normal: $13,200.00</p>
                        <p>Precio Especial: $11,999.00</p>
                        <p class="product-price">Precio al Pagar: $3,000.00-$7,000.00</p>
                    </div>
                    <div class="product">
                        <img src="5.jpg" alt="Producto B">
                        <h3>Soporte para Instrumento Musical </h3>
                        <p class="product-normal-price">Normal: $700.00</p>
                        <p>Precio Especial: $499.00</p>
                        <p class="product-price">Precio al Pagar: $170.00</p>
                    </div>
                    <div class="product">
                        <img src="2.png" alt="Producto C">
                        <h3>Cuadro Personalizable</h3>
                        <p class="product-normal-price">Normal: $800.00</p>
                        <p>Precio Especial: $699.00</p>
                        <p class="product-price">Precio al Pagar: $400.00</p>
                    </div>
                </div>
                </div>
                </div>
                <footer>
                    <div class="footer-section">
                        <h3>ATENCIÓN A CLIENTES</h3>
                        <ul>
                            <li><a href="#estatus-orden">Conoce el estatus de tu orden</a></li>
                            <li><a href="#garantias">Garantías</a></li>
                            <li><a href="tel:5555555555">55 55 55 55 55</a></li>
                        </ul>
                    </div>
                    <div class="footer-section">
                        <h3>TÉRMINOS Y CONDICIONES</h3>
                        <ul>
                            <li><a href="#terminos">Términos y Condiciones</a></li>
                            <li><a href="#aviso-privacidad">Aviso de Privacidad</a></li>
                        </ul>
                    </div>
                    <div class="footer-section">
                        <h3>EXPERIENCIA MOBLUM</h3>
                        <ul>
                            <li><a href="#compra-segura">Compra Segura</a></li>
                            <li><a href="#comunicacion">Comunicación y medios</a></li>
                        </ul>
                    </div>
                    <div class="footer-section">
                        <h3>PROMOCIONES</h3>
                        <ul>
                            <li><a href="#buen-fin">Buen fin</a></li>
                        </ul>
                    </div>
                    <div class="footer-social">
                        <a href="https://wa.me/1234567890"><img src="wasa.png" alt="WhatsApp"></a>
                    </div>
                </footer>
                </body>
                </html>
                
                
