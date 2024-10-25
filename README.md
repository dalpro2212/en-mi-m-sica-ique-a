<!DOCTYPE html>  
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Web Bonita</title>
    <meta name="description" content="Página web de ejemplo con diseño atractivo utilizando HTML y CSS.">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('imagenes/IMAGEN-FONDO.jpg'); 
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
        }
        header {
            background: rgba(53, 66, 74, 0.8);
            padding: 20px 0;
            text-align: center;
        }
        header h1 {
            font-size: 3em;
            font-weight: bold;
            color: #f8f8f4;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
            letter-spacing: 2px;
            margin: 0;
        }
        nav {
            margin: 20px 0;
        }
        nav a {
            color: #ffffff;
            margin: 0 15px;
            text-decoration: none;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        section {
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            margin: 20px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        .tooltip {
            display: none;
            position: absolute;
            background: #35424a;
            color: #ffffff;
            padding: 10px;
            border-radius: 5px;
            z-index: 10;
            left: 320px;
            top: 50%;
            transform: translateY(-50%);
            white-space: nowrap;
        }
        img {
            transition: transform 0.4s linear, box-shadow 0.3s ease;
            margin-right: 20px;
        }
        img:hover {
            transform: scale(1.05);
            box-shadow: 0 0 15px rgba(78, 78, 77, 0.7);
        }
        img:hover + .tooltip {
            display: block;
        }
        .mostrar-mas {
            display: inline-block;
            padding: 10px 15px;
            background-color: #35424a;
            color: #ffffff;
            border-radius: 5px;
            text-decoration: none;
            transition: transform 0.3s ease;
        }
        .mostrar-mas:hover {
            transform: translateY(-3px);
        }
        footer {
            text-align: center;
            padding: 10px 0;
            background: rgba(53, 66, 74, 0.8);
            color: #ffffff;
            position: relative;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

<header>
    <h1>EN MUSICA IQUEÑA</h1>
    <nav>
        <a href="#">Categorías</a>
        <a href="#">Premium</a>
        <a href="servicios.html">Servicios</a> 
        <a href="#">Cuenta</a>
        <a href="eventos.html">Eventos</a> <!-- Enlace a eventos -->
    </nav>
</header>

<div class="container">
    <section>
        <h2>BANDAS</h2>
        <img src="imagenes/IMAGEN-DPOS.jpg" alt="DPOS" style="max-width: 300px; height: 200px;" />
        <div class="tooltip">DPOS es una banda del 2021 que empezó con el pie derecho.</div>
    </section>

    <section>
        <h2>BANDAS EMERGENTES 🎸</h2>
        <div style="display: flex; align-items: center;">
            <img src="imagenes/IMAGEN-ADSEX.jpg" alt="ADSEX" style="max-width: 300px; height: 200px;" />
            <div class="tooltip">Una banda juvenil Iqueña que tiene un proyecto claro en mente, hacer que el rock y pop de los 80s vuelvan a la actualidad. Consta de 7 integrantes.</div>
            <img src="imagenes/IMAGEN-THEENYGMAS.jpg" alt="THEENYGMAS" style="max-width: 300px; height: 200px;" />
            <a href="bandas-emergentes.html" class="mostrar-mas">Mostrar más 🎸</a>
        </div>
    </section>

    <section>
        <h2>EVENTOS 🎹</h2>
        <a href="eventos.html">
            <img src="imagenes/IMAGEN-ARTESANO.jpg" alt="EVENTOS" style="max-width: 300px; height: 200px;" />
        </a>
        <p>DISFRUTA DE LOS MEJORES EVENTOS DE ICA QUE SE VIENEN</p>
    </section>
</div>

<footer>
    <p>&copy; 2024 Mi MUSICA. Todos los derechos reservados.</p>
</footer>

</body>
</html>
