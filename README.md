<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>El Libro Abierto</title>
  <style>
    :root {
      --rosado: #fbb6ce;
      --amarillo: #fff176;
      --marron: #6d1b7b;
      --texto: #333;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff;
      color: var(--texto);
    }

    header {
      background: linear-gradient(to right, var(--rosado), var(--amarillo));
      text-align: center;
      padding: 30px 20px;
    }

    header h1 {
      margin: 0;
      font-size: 2.8em;
      color: var(--marron);
    }

    header p {
      font-style: italic;
      color: #4e1d4f;
      margin-top: 8px;
    }

    nav {
      background-color: var(--amarillo);
      padding: 12px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 25px;
      margin: 0;
      padding: 0;
    }

    nav a {
      text-decoration: none;
      color: var(--marron);
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #a0005c;
    }

    main {
      max-width: 900px;
      margin: auto;
      padding: 40px 20px 100px;
    }

    section {
      margin-bottom: 60px;
      padding-top: 70px;
    }

    h2 {
      color: var(--marron);
      border-bottom: 2px solid #c2185b;
      padding-bottom: 5px;
    }

    ul {
      padding-left: 20px;
    }

    .cuento {
      margin-bottom: 25px;
      padding: 15px;
      background-color: #fffde7;
      border-left: 5px solid var(--rosado);
      border-radius: 6px;
    }

    .button {
      display: inline-block;
      margin-top: 15px;
      background-color: var(--rosado);
      color: var(--marron);
      padding: 10px 20px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
      transition: background-color 0.3s;
    }

    .button:hover {
      background-color: #f48fb1;
    }

    .mascota-img {
      max-width: 200px;
      display: block;
      margin: 20px auto;
      border-radius: 10px;
    }

    .mascota-texto {
      text-align: center;
      font-size: 1.1em;
    }

    footer {
      background-color: var(--rosado);
      text-align: center;
      padding: 15px;
      position: fixed;
      width: 100%;
      bottom: 0;
      color: var(--marron);
    }

    @media (max-width: 600px) {
      nav ul {
        flex-direction: column;
        align-items: center;
      }
    }

    .bandera {
      width: 24px;
      height: 18px;
      vertical-align: middle;
      margin-right: 8px;
    }

    /* Añadido: estilo para la imagen del equipo con efecto zoom */
    .equipo-img {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      transition: transform 0.4s ease;
      display: block;
      margin: 0 auto 20px;
    }

    .equipo-img:hover {
      transform: scale(1.05);
    }
  </style>
</head>
<body>
  <header>
    <h1>The open book</h1>
    <p>Traduciendo saberes, preservando historias</p>
  </header>

  <section id="mascota-bienvenida" style="background-color: #fffce8; padding: 40px 20px; text-align: center;">
    <img src="https://i.imgur.com/xbQKPo1.jpeg" alt="Mascota Libi" class="mascota-img" />
    <div id="dialogo" style="background-color: #fbb6ce; display: inline-block; padding: 15px 20px; border-radius: 20px; max-width: 400px; margin: auto; font-size: 1.1em; color: #4a004d;">
      💬 ¡Hola! Soy <strong>Lexi</strong>, tu compañera en esta aventura de lectura. ¿Listo para descubrir cuentos mágicos?
    </div>
    <br><br>
    <button onclick="responderDialogo()" style="background-color: #fff176; border: none; padding: 10px 20px; border-radius: 10px; font-weight: bold; cursor: pointer;">
      Hablar con Lexi
    </button>
  </section>

  <nav>
    <ul>
      <li><a href="#acerca">Conoce a nuestro equipo</a></li>
      <li><a href="#idiomas">Idiomas</a></li>
      <li><a href="#Lee y descubre">Lee y descubre</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </nav>

  <main>
    <section id="acerca">
      <!-- Añadido: Imagen del equipo -->
      <img src="https://i.imgur.com/EcpOsmw.png" alt="Nuestro equipo" class="equipo-img" />
      <h2>Conoce a nuestro equipo</h2>
      <p>Bienvenidos a The open book, somos un equipo que busca fomentar la igualdad en el aprendizaje garantizando que todos los estudiantes tengan el acceso adecuado a diversos materiales educativos en diferentes idiomas.</p>
    </section>
    <section id="idiomas">
      <h2>Idiomas disponibles</h2>
      <ul style="list-style: none; padding-left: 0;">
        <li><img src="https://flagcdn.com/24x18/pe.png" alt="Perú" class="bandera">Español</li>
        <li><img src="https://flagcdn.com/24x18/pe.png" alt="Perú" class="bandera">Quechua</li>
        <li><img src="https://flagcdn.com/24x18/pe.png" alt="Perú" class="bandera">Aimara</li>
        <li><img src="https://flagcdn.com/24x18/fr.png" alt="Francia" class="bandera">Francés</li>
        <li><img src="https://flagcdn.com/24x18/br.png" alt="Brasil" class="bandera">Portugués</li>
        <li><img src="https://flagcdn.com/24x18/gb.png" alt="Inglaterra" class="bandera">Inglés</li>
        <li><img src="https://flagcdn.com/24x18/it.png" alt="Italia" class="bandera">Italiano</li>
     </ul>
    </section>

    <section id="Lee y descubre">
      <h2>Lee y descubre</h2>

      <div class="Lee y descubre">
        <h3>🙏 El sacerdote sin cabeza</h3>
        <p>Un relato espeluznante que cuenta la historia de un religioso decapitado que vaga en busca de redención, generando terror en quienes lo ven. Su presencia anuncia desgracias y muerte.</p>
      </div>

      <div class="Lee y descubre">
        <h3>🏠 La casa Musita</h3>
        <p>Una leyenda piurana que narra hechos misteriosos ocurridos en una antigua casona. Relata sucesos paranormales, apariciones y ruidos inexplicables, que han despertado temor y curiosidad en los pobladores, convirtiéndola en parte del folclore local.</p>
      </div>

      <div class="Lee y descubre">
        <h3>😭 La llorona </h3>
        <p>Cuenta la historia de una mujer que ahogó a sus hijos en un río tras ser abandonada por su amante, y ahora vaga llorando y buscando a sus hijos, generando miedo en quienes la escuchan.</p>
      </div>

      <p>👉 También puedes explorar más cuentos a tu idioma:
        <a class="button" href="https://beamish-paletas-493432.netlify.app/" target="_blank">Ver The open book</a>
      </p>
    </section>

    <section id="contacto">
      <h2>Contacto</h2>
      <p>Escríbenos a: <a href="mailto:@The_open_book.com">theopenbook.original@gmail.com</a></p>
      <p>🌐 Proyecto:
        <a href="https://beamish-paletas-493432.netlify.app/" target="_blank">The open book</a>
      </p>
    </section>
  </main>

  <footer>
    © 2025 The open book. Todos los derechos reservados.
  </footer>

  <script>
    let mensajes = [
      "¿Quieres leer un cuento mágico o aprender una palabra nueva?",
      "Recuerda: ¡Leer en tu idioma fortalece tu identidad! 😊",
      "Estoy aquí para ayudarte a explorar nuevos mundos con tus palabras favoritas.",
      "¡Explora los cuentos más abajo y dime cuál te gusta más!"
    ];
    let i = 0;

    function responderDialogo() {
      const dialogo = document.getElementById("dialogo");
      dialogo.innerHTML = "💬 " + mensajes[i];
      i = (i + 1) % mensajes.length;
    }
  </script>

</body>
</html>

