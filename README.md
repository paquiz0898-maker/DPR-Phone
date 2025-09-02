<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>DPR Phone - Recuperación de Datos</title>
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #fff; color: #333;
    }
    /* Header */
    header {
      background: #ff6600; color: white;
      padding: 15px 30px;
      display: flex; align-items: center; justify-content: space-between;
      position: sticky; top: 0; z-index: 10;
    }
    header img { height: 60px; }
    nav a { color: white; text-decoration: none; margin-left: 20px; font-weight: bold; }
    nav a:hover { text-decoration: underline; }

    nav a.contacto {
      background: #25D366; color: white !important;
      padding: 8px 15px; border-radius: 5px;
      display: inline-flex; align-items: center; gap: 6px;
    }
    nav a.contacto:hover { background: #1ebe57; }

    /* Hero */
    .hero {
      background: linear-gradient(rgba(255,102,0,0.6), rgba(255,102,0,0.6)),
                  url("Dpr01.PNG") center/cover no-repeat;
      color: white;
      text-align: center;
      padding: 100px 20px;
    }
    .hero h1 { font-size: 3em; margin-bottom: 10px; }
    .hero p { font-size: 1.3em; margin-bottom: 20px; }
    .hero a.cta {
      background: white; color: #ff6600; padding: 12px 25px;
      text-decoration: none; font-weight: bold; border-radius: 5px;
    }
    .hero a.cta:hover { background: #f0f0f0; }

    /* Cards */
    .servicios {
      display: flex; justify-content: center; flex-wrap: wrap;
      margin: 40px auto; max-width: 1200px;
    }
    .card {
      background: white; border-radius: 10px; width: 250px;
      margin: 15px; padding: 20px;
      box-shadow: 0px 4px 8px rgba(0,0,0,0.2);
      text-align: center; transition: transform 0.2s;
    }
    .card:hover { transform: scale(1.05); }
    .card h2 { color: #cc5200; }
    .precio { font-size: 1.6em; font-weight: bold; color: #ff6600; }
    .btn {
      display: inline-block; margin-top: 15px;
      padding: 10px 20px; background: #ff6600;
      color: white; text-decoration: none; border-radius: 5px;
    }
    .btn:hover { background: #cc5200; }

    /* Redes */
    .card .social-links a {
      margin: 10px; font-size: 1.8em;
      color: #ff6600; transition: color 0.3s;
    }
    .card .social-links a:hover { color: #cc5200; }

    /* Testimonios */
    .testimonios { background: #f9f9f9; padding: 50px 20px; }
    .testimonios h2 { text-align: center; color: #ff6600; margin-bottom: 30px; }
    .testimonios .card { width: 300px; font-style: italic; }

    /* FAQ */
    .faq { padding: 50px 20px; }
    .faq h2 { text-align: center; color: #ff6600; margin-bottom: 30px; }
    .faq details { margin: 10px auto; max-width: 700px; background: #f2f2f2; padding: 15px; border-radius: 5px; }
    .faq summary { font-weight: bold; cursor: pointer; }

    /* Footer */
    footer { margin-top: 40px; padding: 20px; background: #ff6600; color: white; text-align: center; }

    /* WhatsApp flotante */
    .whatsapp-float {
      position: fixed; width: 60px; height: 60px;
      bottom: 20px; right: 20px;
      background: #25D366; color: white;
      border-radius: 50%; font-size: 30px;
      display: flex; align-items: center; justify-content: center;
      box-shadow: 2px 2px 5px rgba(0,0,0,0.3);
      z-index: 100; transition: background 0.3s; animation: bounce 1.8s infinite;
    }
    .whatsapp-float:hover { background: #1ebe57; }

    /* Llamada flotante */
    .call-float {
      position: fixed; width: 60px; height: 60px;
      bottom: 100px; right: 20px;
      background: #007bff; color: white;
      border-radius: 50%; font-size: 28px;
      display: flex; align-items: center; justify-content: center;
      box-shadow: 2px 2px 5px rgba(0,0,0,0.3);
      z-index: 100; transition: background 0.3s;
    }
    .call-float:hover { background: #0056b3; }

    /* Animación */
    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
      40% { transform: translateY(-10px); }
      60% { transform: translateY(-5px); }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <img src="logo_dprphone.png" alt="DPRPhone Logo">
    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#servicios">Servicios</a>
      <a href="#otros-servicios">Otros Servicios</a>
      <a href="#about">Acerca de Nosotros</a>
      <a href="#faq">FAQ</a>
      <a href="#contacto" class="contacto"><i class="fab fa-whatsapp"></i> Contacto</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero" id="inicio">
    <h1>DPRPhone</h1>
    <p>Especialistas en Recuperación de Datos de Teléfonos</p>
    <a href="#otros-servicios" class="cta">Ver Servicios</a>
  </section>

  <!-- Servicios -->
  <section class="servicios" id="servicios">
    <div class="card"><h2>VIP</h2><p class="precio">$4,700</p><p>Máxima seguridad y velocidad.</p><a href="https://wa.me/524612574352?text=Hola,%20quiero%20VIP%20📱" target="_blank" class="btn">Solicitar</a></div>
    <div class="card"><h2>Gama Alta</h2><p class="precio">$3,500</p><p>Recuperación avanzada premium.</p><a href="https://wa.me/524612574352?text=Hola,%20quiero%20gama%20alta%20📱" target="_blank" class="btn">Solicitar</a></div>
    <div class="card"><h2>Gama Media</h2><p class="precio">$2,200</p><p>Confiable para equipos estándar.</p><a href="https://wa.me/524612574352?text=Hola,%20quiero%20gama%20media%20📱" target="_blank" class="btn">Solicitar</a></div>
    <div class="card"><h2>Gama Baja</h2><p class="precio">$1,200</p><p>Económico para dispositivos básicos.</p><a href="https://wa.me/524612574352?text=Hola,%20quiero%20gama%20baja%20📱" target="_blank" class="btn">Solicitar</a></div>
    <div class="card" id="about">
      <h2>Acerca de Nosotros</h2>
      <p>En <b>DPRPhone</b> somos especialistas en recuperación de datos de teléfonos móviles de todas las gamas.</p>
      <div class="social-links">
        <a href="https://www.instagram.com/dpr_phone" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://www.tiktok.com/@dprphone" target="_blank"><i class="fab fa-tiktok"></i></a>
      </div>
    </div>
  </section>

  <!-- Otros Servicios -->
  <section class="otros-servicios" id="otros-servicios">
    <h2 style="text-align:center; color:#ff6600; margin-top:50px;">Otros Servicios</h2>
    <div class="servicios">
      <div class="card"><h2>Restauración</h2><ul style="text-align:left;"><li>🔧 Pantalla</li><li>🔋 Batería</li><li>🔊 Parlantes</li><li>⚡ Carga</li></ul></div>
      <div class="card"><h2>Micro soldadura</h2><ul style="text-align:left;"><li>🔬 Reballing</li><li>🔄 Swap</li><li>🛠️ Otros</li></ul></div>
      <div class="card"><h2>Software</h2><ul style="text-align:left;"><li>🤖 Android</li><li>🍏 iOS</li><li>🖥️ Windows</li><li>💻 MacOS</li></ul></div>
    </div>
  </section>

  <!-- Testimonios -->
  <section class="testimonios">
    <h2>Lo que dicen nuestros clientes</h2>
    <div class="servicios">
      <div class="card"><p>"Me recuperaron todas mis fotos, pensé que las había perdido para siempre. ¡Recomendados!"</p><strong>- Juan P.</strong></div>
      <div class="card"><p>"Excelente servicio, rápido y seguro. Ya es mi centro de confianza."</p><strong>- María L.</strong></div>
    </div>
  </section>

  <!-- FAQ -->
  <section class="faq" id="faq">
    <h2>Preguntas Frecuentes</h2>
    <details><summary>¿Cuánto tarda la recuperación?</summary><p>Generalmente entre 24 y 72 horas, dependiendo del daño.</p></details>
    <details><summary>¿Qué pasa si no se recuperan los datos?</summary><p>No se cobra el servicio, aplicamos política de no recuperación = no pago.</p></details>
    <details><summary>¿Atienden equipos mojados?</summary><p>Sí, contamos con tratamiento especial para humedad y líquidos.</p></details>
  </section>

  <!-- Contacto -->
  <section class="contacto" id="contacto">
    <h2 style="text-align:center; color:#ff6600;">Contáctanos</h2>
    <div style="text-align:center; margin-bottom:30px;">
      <p>📱 Escríbenos por WhatsApp:</p>
      <a href="https://wa.me/524612574352?text=Hola,%20quiero%20cotizar%20mi%20equipo%20📱💻" target="_blank" class="btn">+52 461 257 4352</a>
    </div>
    <div style="max-width: 800px; margin: 20px auto; border-radius: 10px; overflow: hidden; box-shadow: 0px 4px 10px rgba(0,0,0,0.3);">
      <iframe 
  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3733.191053973595!2d-100.808838!3d20.528388!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x842cba9ad38b48b5%3A0x2a19fca472f4fc3e!2sNuevo%20Le%C3%B3n%20404%2C%20Alameda%2C%2038050%20Celaya%2C%20Gto.!5e0!3m2!1ses-419!2smx!4v1693600000000" 
  width="100%" height="400" 
  style="border:0;" 
  allowfullscreen="" 
  loading="lazy" 
  referrerpolicy="no-referrer-when-downgrade">
</iframe>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>📞 Tel: +52 461 257 4352 | ✉️ soporte@dprphone.com</p>
    <p>&copy; 2025 DPRPhone - Todos los derechos reservados</p>
  </footer>

  <!-- Botones flotantes -->
  <a href="https://wa.me/524612574352?text=Hola,%20quiero%20cotizar%20mi%20equipo%20📱💻" class="whatsapp-float" target="_blank"><i class="fab fa-whatsapp"></i></a>
  <a href="tel:+524612574352" class="call-float"><i class="fas fa-phone"></i></a>

</body>
</html>
